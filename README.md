# My build of dwm

https://dwm.suckless.org/

See also
* [my st build](https://github.com/lnhrnndz/st)
* [my dmenu build](https://github.com/lnhrnndz/dmenu)
* [my dotfiles](https://github.com/lnhrnndz/dotfiles)

## Installation
Clone and build dwm
``` bash
git clone https://github.com/lnhrnndz/dwm
cd dwm
sudo make install
```
Add the following at the bottom of your `.xinitrc`
``` bash
exec dbus-run-session dwm
```
Start X
``` bash
startx
```
Exit with
``` bash
pkill dwm
```

## Keybindings

| keybinding                         | description                                          |
| ---------------------------------- | ---------------------------------------------------- |
| `super + shift + return`           | spawn new [st](https://github.com/lnhrnndz/st)    |
| `super + p`                        | run [dmenu](https://github.com/lnhrnndz/dmenu)       |
| `super + j\|k`                     | focus window below or above on stack                 |
| `super + shift + j\|k`             | move focused window down or up the stack             |
| `super + return`                   | swap master and focused window                       |
| `super + [1..n]`                   | view all windows with nth tag                        |
| `super + shift + [1..n]`           | apply nth tag to focused window                      |
| `super + control + [1..n]`         | add/remove all windows with nth tag to/from the view |
| `super + shift + control + [1..9]` | add/remove tag to focused window                     |
| `super + shift + space`            | toggle window floating                               |
| `super + [arrow key]`              | move floating window                                 |
| `super + shift + [arrow key]`      | resize floating window                               |
| `super + t`                        | tiling layout                                        |
| `super + m`                        | monocle layout                                       |
| `super + f`                        | floating layout                                      |
| `super + r`                        | deck layout                                          |
| `super + y`                        | toggle fullscreen mode                               |
| `super + shift + [arrow key]`      | resize floating window                               |
| `super + F5`                       | reload colors form xresources                        |
| `super + shift + r`                | reload dwm (without quitting)                        |

## Patches

* [gaps](https://dwm.suckless.org/patches/gaps/)
* [attachbottom](https://dwm.suckless.org/patches/attachbottom/)
* [pertag](https://dwm.suckless.org/patches/pertag/)
* [movestack](https://dwm.suckless.org/patches/movestack/)
* [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/)
* [moveresize](https://dwm.suckless.org/patches/moveresize/)
* [restartsig](https://dwm.suckless.org/patches/restartsig/)
* [xrdb](https://dwm.suckless.org/patches/xrdb/)
* [togglefullscreen](https://github.com/bakkeby/patches/blob/master/dwm/dwm-togglefullscreen-6.2.diff)
* [deck layout](https://dwm.suckless.org/patches/deck/) (+ deck-tilegap)

## Desktop entry

Edit and move `xinit.desktop` to `/usr/share/xsessions/` to have a desktop entry
that runs your `.xinitrc`.
