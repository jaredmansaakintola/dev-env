# dev-env
Docker Development Environment (Using ansible provisioner)

Manage Docker as non-root user:

Create the docker group.

$ sudo groupadd docker
Add your user to the docker group.

$ sudo usermod -aG docker $USER
Log out and log back in so that your group membership is re-evaluated.

If testing on a virtual machine, it may be necessary to restart the 
virtual machine for changes to take effect.

On a desktop Linux environment such as X Windows, log out of your session completely and then log back in.

Verify that you can run docker commands without sudo.

$ docker run hello-world

# INCASE OF EMERGENCY BREAK

Remove rm -f /var/lib/linkpgraph.db (or if you modified graphdb=/opt/docker : rm -rf /opt/docker/linkgraph.db)
Remove rm -rf /var/lib/containers/
Restart docker daemon : (for Ubuntu) sudo service docker restart


