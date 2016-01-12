# Registry

This catalogue item consists of a Registry, and the Portus web UI for 
authentication.  There is also a MySQL database for storage, and a nginx
proxy to provide SSL for the web frontend.

## Backing Store

A persistent shared filesystem is required to host the Registry, and also the 
MySQL database.  This will also hold the certificates under certs/server.crt
and certs/server.key; if no certificate is present, then a self-signed
certificate will be created (valid for one year only) that can later be 
replaced.

## LDAP Authentication

If you enable LDAP authentication, then this will be used for both the
Web interface and for Registry authentication.  The LDAP configuration
may optionally have authenticated Bind credentials, and TLS options.

## Administration

The first user to log in to the web interface will be granted Admin
privileges.

