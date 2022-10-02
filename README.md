# My build of dwm

https://dwm.suckless.org/

## Keybindings

| keybinding                    | description                      |
| ----------------------------- | -------------------------------- |
| `super + F5`                  | reload colors form xresources    |
| `super + y`                   | toggle fullscreen mode           |
| `super + shift + space`       | toggle window floating           |
| `super + [arrow key]`         | move floating window             |
| `super + shift + [arrow key]` | resize floating window           |
| `super + r`                   | deck layout                      |
| `super + shift + j\|k`        | move window up or down the stack |

## Patches

- [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/)
- [attachbottom](https://dwm.suckless.org/patches/attachbottom/)
- [gaps](https://dwm.suckless.org/patches/gaps/)
- [moveresize](https://dwm.suckless.org/patches/moveresize/)
- [restartsig](https://dwm.suckless.org/patches/restartsig/)
- [togglefullscreen](https://github.com/bakkeby/patches/blob/master/dwm/dwm-togglefullscreen-6.2.diff)
- [xrdb](https://dwm.suckless.org/patches/xrdb/)
- [pertag](https://dwm.suckless.org/patches/pertag/)
- [deck layout](https://dwm.suckless.org/patches/deck/) (+ deck-tilegap)
- [movestack](https://dwm.suckless.org/patches/movestack/)

## Desktop entry

Edit and move xinit.desktop to /usr/share/xsessions/ to have a desktop entry
that runs your .xinitrc.
