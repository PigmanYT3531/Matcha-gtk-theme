## Disclaimer
- This is an unofficial fork of Matcha GTK Theme
- Donate button is removed because it's irrelevant here
- If you want to donate to the original repo, well, just go to the original repo


<img src="https://github.com/vinceliuice/matcha/blob/imgs/logo.png" alt="Logo" align="right" /> Matcha Gtk Theme
======

Matcha is a flat Design theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Unity, Budgie, Pantheon, XFCE, Mate, etc.

This theme is based on Arc gtk theme of horst3180. Thanks horst3180 sincerely for his great job!

horst3180 - Arc gtk theme: https://github.com/horst3180/Arc-theme

## Info

### GTK+ > 3.20

### GTK2 engines requirment
- GTK2 engine Murrine 0.98.1.1 or later.
- GTK2 pixbuf engine or the gtk(2)-engines package.

Fedora/RedHat distros:

    yum install gtk-murrine-engine gtk2-engines

Ubuntu/Mint/Debian distros:

    sudo apt-get install gtk2-engines-murrine gtk2-engines-pixbuf

ArchLinux:

    pacman -S gtk-engine-murrine gtk-engines

Solus:

    sudo eopkg it gtk2-engine-murrine gtk-engines

Other:
Search for the engines in your distributions repository or install the engines from source.

## Install

### Install from source file

Double-click to open that script file,
Or open the terminal at current directory.

Run

    ./install.sh -c dark

Usage: ./install.sh [OPTIONS...]

OPTIONS:

```sh
  -d, --dest DIR           Specify theme destination directory (Default: /home/fedora/.themes)
  -n, --name NAME          Specify theme name (Default: Matcha)
  -c, --color VARIANTS     Specify theme color variant(s) [standard|dark] (Default: All variants)
  -t, --theme VARIANTS     Specify hue theme variant(s) [aliz|azul|sea|pueril] (Default: All variants)
  -s, --gnome-shell        Set gnome-shell flavor, where new is version 44.0 or later, [38|40|42|44] (Default: Auto detect)
  -l, --libadwaita         Force all libadwaita app use linked gtk-4.0 theme
  -g, --gdm                Install GDM theme, this option need root user authority! please run this with sudo
  -r, --remove             Remove(Uninstall) themes/GDM/libadwaita
  -h, --help               Show this help
```

### Fix for flatpak apps

    sudo flatpak override --filesystem=~/.themes

If you installed your theme in system theme folder then run:

    sudo flatpak override --filesystem=/usr/share/themes
