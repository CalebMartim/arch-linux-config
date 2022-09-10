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
- rofi

    Task runner
- pulseaudio and alsa-utils

    For audio configuration
- fish

    Shell 
- ranger

    File management



## Useful programs
- code

    Programming
- gimp

    Image editing
- lxappearance

    For setting GTK themes


# Nice to have programs
- pfetch

    Minimalist system info display

- peaclock

    Minimalist clock on terminal window

- cava

    Terminal audio visualizer

## Observations
Use `$ xdg-mime default firefox.desktop x-scheme-handler/https x-scheme-handler/http` to make Firefox the default browser
