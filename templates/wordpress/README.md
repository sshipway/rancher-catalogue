# Wordpress

### Topology

This will start up a single database instance, and multiple WordPress
servers using it.  Load balancers will be started over the multiple
Wordpress instances.

The load balancers will run on every host with the label **LB=1**.  If
no hosts match this, then you will get no load balancers!

### Options

You should specify a unique port number for the load balancers to listen on.

You need to create a new password for the database user.  Do not make this
obvious.

The first time that you visit the Wordpress server, you will be asked to 
configure a user.

