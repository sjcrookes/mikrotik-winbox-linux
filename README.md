# MikroTik Winbox on Linux
How to install MikroTik's Winbox device management interface on Linux

## Install Dependancies
* You will need an x11 display, Wayland support is apparently limited as at 2024-10

### Debian 12
```
apt install unzip libxcb-xkb1 libxkbcommon-x11-0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-render-util0
```

## Download Winbox Linux 64bit from MikroTik website
[https://mikrotik.com/download](https://mikrotik.com/download)

## Extract and run as normal user
```
unzip -d winbox Winbox_Linux.zip
cd winbox
./WinBox
```

## Failing to run
* Run from the command line to see if there are any errors
* Run ```ldd Winbox``` to see what libraries it requires and is missing
