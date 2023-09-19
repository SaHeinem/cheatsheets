# tmux Cheatsheet
this document is intended as reference for some tmux commands. The author does not claim completeness

## Table of contents
* [Autostart in ZSH](#autostart-in-zsh)
* [Window](#window)
* [Panes](#panes)

## Autostart in ZSH
add this to your `.zshrc` file:
````sh
if [ "$TMUX" = "" ]; then tmux; fi
````

## Window
|Shortcut|Effect|
|---|---|
|Ctrl + b c|create new window|
|Ctrl + b ,|rename current window|
|Ctrl + b &|close window|
|Ctrl + b w|list windows|
|Ctrl + b p|previous|
|Ctrl + b n|next|
|Ctrl + b 0..9|go to number|
|Ctrl + b l|last active|


## Panes
|Shortcut|Effect|
|---|---|
|Ctrl + b ;|last active pane|
|Ctrl + b %|new horizontal|
|Ctrl + b "|new vertical|
|Ctrl + b ←/→|use left right or up down pane|
|Ctrl + b {/}|move left / right|
|Ctrl + b !|convert pane to window|

### Open Pane in same directory
edit your `.tmux.conf` file:
````
# Set new panes to open in current directory
bind c new-window -c "#{pane_current_path}"
bind '"' split-window -c "#{pane_current_path}"
bind % split-window -h -c "#{pane_current_path}"
````
