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

Then, use `wp --choose` to display all your wallpapers and choose one.
You can alternatively use a file name query - let's say you have these wallpapers: `wallpaper-forest.png`, `wallpaper-city.png`, `wallpaper-sky.png` and you want to set `wallpaper-forest.png` as you wallpaper, you can basically do `wp --choose forest` and `wp` will look for any wallpapers with `forest` in their name, if there is multiple wallpapers like that, it will let you choose one.

If you love all your wallpapers and don't know which one to pick, use `wp --random` which will randomly pick you a wallpaper.

If you want your wallpaper to change every 10 seconds, you can use `wp --loop` to do that.

### Disclaimer

If you set wallpaper with `wp`, once you reboot your changes will be lost.
If you want them to remain, add this to your i3 `config` file:

```
exec_always --no-startup-id wp --choose my-favorite-wallpaper.png
```
