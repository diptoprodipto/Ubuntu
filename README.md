# Ubuntu
> All about Ubuntu/Linux commands

## 20 things to do after fresh installation
- Resource: https://www.youtube.com/watch?v=GrI5c9PXS5k

## Install Ubuntu Restricted Extras

```bash
sudo apt install ubuntu-restricted-extras
```

## Minimize on click
### Enable

``` bash
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize-or-previews'
```

### Disable

``` bash
gsettings reset org.gnome.shell.extensions.dash-to-dock click-action
```

### Checking all avilable commands

``` bash
gsettings range org.gnome.shell.extensions.dash-to-dock click-action
```

- Resource: https://itsfoss.com/click-to-minimize-ubuntu/
- Resource: https://askubuntu.com/questions/1026442/how-can-i-hover-over-icons-in-ubuntu-dock-to-see-all-windows-of-one-application

## Download GitHub Desktop
- Resource: https://github.com/shiftkey/desktop#debianubuntu-distributions

## Download GCC & C/C++ dependencies
```bash
sudo apt install build-essential
```

## Run C programs on terminal
```bash
- touch hello.c
- nano hello.c
- gcc hello.c -o hello.out
- ./hello.out
```

## Booting problem: BusyBox v1.30.1 / initramfs
- Check the file system and find the partition name in which Ubuntu is installed.
- Run the following command on the BusyBox terminal.

```bash
fsck -f /dev/<your-drive>
```
- Resource: https://askubuntu.com/questions/1351906/booting-problem-busybox-v1-30-1-initramfs
- Resource: https://askubuntu.com/questions/953728/how-to-check-a-filesystem-in-ubuntu-16-04

## Customize dock panel using dconf-editor
- Install dconf-editor by the following command:

```bash
sudo apt install dconf-editor
```

- For customizing the dock open dconf-editor and go to the following path:

```bash
org/gnome/shell/extensions/dash-to-dock/
```
- Resource: https://www.youtube.com/watch?v=2bCHAOr0Hdg

## Adding Open as Administrator on right click

```bash
- sudo apt install nautilus-admin
- nautilus -q
```

## Adding permission to restricted folder

```bash
sudo chmod -R 777 /opt/lampp/htdocs
```
- Resource: https://www.computernetworkingnotes.com/linux-tutorials/xampp-htdocs-permission-issue-and-fix-in-ubuntu.html
- Resource: https://askubuntu.com/questions/642744/read-write-permissions-in-opt-directory

## Adding solid color wallpaper

```bash
gsettings set org.gnome.desktop.background primary-color '#2c001e'
```
- Resource: https://connectwww.com/change-ubuntu-background-to-solid-colour-set-wallpaper-to-solid-color-in-ubuntu/62142/

## Install failed to install packages/dependencies

```bash
sudo apt --fix-broken install
```