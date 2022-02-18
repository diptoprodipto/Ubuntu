# Ubuntu
> All about Ubuntu/Linux commands

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


