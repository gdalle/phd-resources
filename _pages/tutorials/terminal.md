---
permalink: /tutorials/terminal/
title: Terminal
subtitle: I'll be bash...
sidebar:
    nav: "tutorials"
---

> Work in progress

Roadmap:

- basic bash commands and navigation
- SSH connections
- multiplexing with tmux

## SSH commands

### Connecting

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

### Mounting

```shell
sshfs server:/.../some_folder ~/.../some_folder
```

Unmounting can be performed in the file explorer.


## Multiplexing with tmux

Tmux enables you to run several terminals in parallel. Setting the following parameters in `~ /.tmux.conf` (adapted from http://denisrosenkranz.com) makes the interface more intuitive.

```bash
# Mouse scrolling
set -g mouse on

# Ctrl + arrows to navigate between terminals
bind-key -n C-right next
bind-key -n C-left prev

# Alt + arrows to navigate between terminals
bind-key -n M-left select-pane -L
bind-key -n M-right select-pane -R
bind-key -n M-up select-pane -U
bind-key -n M-down select-pane -D

# Natural shortcuts for vertical and horizontal splits
bind | split-window -h
bind - split-window -v

# Grey for non-active panels
set -g pane-border-fg colour255
set -g pane-border-bg default

# Blue for active panel
set -g pane-active-border-fg colour81
set -g pane-active-border-bg default

# Blue for status bar
set -g status-fg colour0
set -g status-bg colour81
set -g status-attr dim
```

