# Tmux

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
