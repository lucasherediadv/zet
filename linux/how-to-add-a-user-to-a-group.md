Use the following command, replacing `groupname` with the actual group and `username` with the target user's name:

```sh
sudo usermod -aG groupname username
```

How to verify the change:

```sh
groups username
```

For the user's new group membership to take effect, they must log out and log back in to their shell or desktop environment.

If the user is currently logged in and you want the change to apply immediately without logging out, you can have them run the following command to start a new shell session with the updated group information:

```sh
newgrp groupname
```
