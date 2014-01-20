Change chroot dir to your directory (can't use absolute paths for the
map for some reason).

Start server, connect to haproxy socket, then run:

    show map

Should see domain.map listed.  Then run:

    add map domain.map <hostname> <backend>

The new route should be live immediately.
