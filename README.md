# arch-linux-config
My configuration files for my custom Arch Linux build
![](https://cdn.discordapp.com/attachments/326901357300678657/1018289234618093668/Screenshot_archlinux_2022-09-10_193619.png)

## Base system packages
- **xf86-video-amdgpu** 

    For graphics card drivers. (use xf86-video-intel if using an intel cpu)
- **xorg**

    Display server
- **xorg-xinit**

    For starting the xorg display server
- **xdg-utils**

    Program that helps integrate applications and your desktop. It helps adding a default browser for example.
- **git**

	Git
- **paru**

	AUR helper 
- **picom**

    Compositor
- **bspwm**

    Tiling window manager
- **sxhkd**

    Program used for key binds
- **feh**

    For image viewing and wallpaper setting
- **alacritty**

    Terminal emulator
- **polybar**

    Status bar
- **ranger**

    File management
- **rofi**

    Task runner
- **pulseaudio** and **alsa-utils**

    For audio configuration
- **fish**

    Shell program




## Useful packages
- **code**

    Programming
- **gimp**

    Image editing
- **lxappearance**

    For setting GTK themes
- **unzip** and **zip**

	to zip and unzip files


## Nice to have packages
- **pfetch**

    Minimalist system info display
- **peaclock**

    Minimalist clock on terminal window
- **moc**
	Music player on terminal (open with `$ mocp`) 
- **cava**

    Terminal audio visualizer
- **fortune**

    Makes an animal tell you a motivating phrase when running `cowfortune`


## Observations
Use `$ xdg-mime default firefox.desktop x-scheme-handler/https x-scheme-handler/http` to make Firefox the default browser

Run `$ rofi-theme-selector` to apply the gruvbox-dark-soft theme

To set up the gtk theme, you will download the theme at the link on the themes list, unzip the .zip file at the `~/.themes` directory and select that theme on lxappearance and hit "Apply"

To set up a moc theme, first open moc and type T to open the themes tab, remember the name of your favorite theme and on the terminal do: `$ echo "Theme = *your theme* > ~/.moc/config`  

To enable drag and drop in Ranger install dragon-drop from the AUR; Create Ranger config files by typing `$ ranger --copy-config=all` and on the rc.conf file add this line:

	map <C-d> shell dragon-drop -a -x %p --and-exit
Now when you select a file and press ctrl + d, it will enable you to drag and drop it somewhere

To make fish the default shell, do:
	
	echo /usr/local/bin/fish | sudo tee -a /etc/shells
	chsh -s /usr/local/bin/fish
