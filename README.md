# arch-linux-config
My configuration files for my custom Arch Linux build

## Base system programs
- xf86-video-amdgpu 

    For graphics card drivers. (use xf86-video-intel if using an intel cpu)
- xorg

    Display server
- xorg-xinit

    For starting the xorg display server
- xdg-utils

    Program that helps integrate applications and your desktop. It helps adding a default browser for example. 
- picom

    Compositor
- bspwm

    Tiling window manager
- sxhkd

    Program used for key binds
- feh

    For image viewing and wallpaper setting
- alacritty

    Terminal emulator
- polybar

    Status bar

## Other programas
- code

    Programming
- gimp

    Image editing

## Observations
Use `$ xdg-mime default firefox.desktop x-scheme-handler/https x-scheme-handler/http` to make Firefox the default browser