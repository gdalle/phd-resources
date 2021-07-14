# SSH

## Connecting

```shell
ssh username@server.com
```

### No username, server adress or jump

In the file `.ssh/config`, write:

```
Host server
  HostName server.com
  User username
  ProxyJump proxy_server
```

### No password

```shell
ssh-keygen
ssh-copy-id -i ~/.ssh/id_rsa.pub username@server.com
```

## Mounting

```shell
sshfs server:/.../some_folder ~/.../some_folder
```

Unmounting can be performed in the file explorer.
