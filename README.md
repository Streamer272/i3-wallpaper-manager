# i3 WallPaper manager

Lightweight i3 wallpaper manager written in bash

## Installation

### Requirements

- `feh`
- `zsh`

Install `wp`

```
curl https://raw.githubusercontent.com/Streamer272/i3-wallpaper-manager/main/wp -o /usr/bin/wp && chmod +x /usr/bin/wp
```

## Quick start

Create `~/.config/i3/wallpapers` directory and put all your wallpapers there.

Enter `wp --help` to see all available commands

### Disclaimer

If you set wallpaper with `wp`, once you reboot your changes will be lost.
If you want them to remain, add this to your i3 `config` file:

```
exec_always --no-startup-id wp --choose my-favorite-wallpaper.png
```
