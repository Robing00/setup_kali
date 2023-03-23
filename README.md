# Kali-Clean

This is a guide for installing Kali Linux with additional programs and configurations, including a clean i3 desktop installation using the provided [install_i3.sh](../main/install_i3.sh) or [install.sh(without i3)](main/install.sh) script, which contains configuration settings for alacritty and i3 by [xct](https://github.com/xct). 

main/install_i3.sh

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
