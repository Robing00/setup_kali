# Kali-Clean

This is a guide for installing Kali Linux with additional programs and configurations, including a clean i3 desktop installation using the provided [install_i3.sh](../main/install_i3.sh) or [install.sh (if you dont want to use i3)](../main/install.sh) script, which contains configuration settings for alacritty and i3 by [xct](https://github.com/xct). 

## Installation
To begin the installation, clone the repository and execute ./install.sh as a non root user. It will update Kali and install various packages, although it may take some time to complete.

```
./install.sh
```

## Installation for i3

```
./install_i3.sh
```


After the script has finished running, reboot your system and select i3 from the top right corner of the login screen. Then, open a terminal using the shortcut ctrl+return, run the command lxappearance, and choose the ark-dark theme, and customize the icons as desired, such as using papyrus.

## Additional Informations
### Tmux
Inside the [tmux configuration file](../main/.config/tmux/.tmux.conf) there are a few changes to the normal installation like colors and keyboard shortcuts.
#### controls
The contoles are changed for "ctrl+b" to "ctrl+a".
Here is a little Cheatsheet for the most important controls:
- C + a + %       -> new pane
- C + a + "
- C + a + o       -> switch pane
- C + a + c       -> new tab 
- C + a + 1,2,3.. -> switch tab
- C + a + ,       -> rename
- C + a + &       -> close window

The support for mouse switching panes/windows is enables. If you have Problems with it just comment out the "set -g mouse on" inside the [.conf](../main/.config/tmux/.tmux.conf) file.

If you want to have hjkl pane traversal like in vim, just add the following to the [config file](../main/.config/tmux/.tmux.conf):<br>
```
bind h select-pane -L
bind j select-pane -D
bind k select-pane -U
bind l select-pane -R
```
