# xfce4-wayland-arch
testing repo for running xfce4 + labwc on wayland (currently only managed to do it in arch)

*uses chicago95 theme: https://github.com/grassmunk/Chicago95* , the menu shortcut is Super + S currently.

run makepkg -si in all folders except labwc, put that in your .config folder, theme used in the labwc config is chicago95, install that if you like or dont wanna learn how to mess with the labwc config, also install labwc (not auto installed rn), gsettings-desktop-schemas and waypaper + swaybg for your wallpapers (default xfce wallpaper setting app works, but has a few noticeable bugs, such as: if you enable "reserve space on screen edges for the panel" in panel settings, and make you panel's lenth lower than max, there will be black bars in the free space of the panel; it also for some reason doesnt totally apply on boot, it launches but only shows after you change resolution)

**IMPORTANT** the keyboard variant is colemak by default, which you probably dont use, edit ~/.config/labwc/environment and remove the XKB_DEFAULT_VARIANT=colemak, just removing it should make it go back to qwerty, of course you should restart the desktop for it to apply, since its a env variable

use _startxfce4 --wayland_ to start from tty, your display manager will probably show a desktop entry for it tho 
