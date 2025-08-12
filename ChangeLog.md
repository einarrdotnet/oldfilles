# Arch Linux Post Install Change Log

The following documentation is a Arch Linux post install change log where i have extensivly documented ever change i have made to my base install of Arch Linux.

## Preinstall Notes

During the fresh installation of Arch Linux the following packages were installed through the "packstrap" command
    -Base
    -base-devel
    -linux
    -linux-firmware
    -networkmanager
    -grub (grub system bootloader)
    -efibootmgr (required dependice for grub)
    -neovim (terminal based text editor of choice reqired for installtion)

## Setting up a Working Enviroment

after rebooting into the fresh install of Arch Linux and logging into the tty with the user created during the install i needed to setup a working enviroment

### Bash Customisation

In order to make the process of setting up a working enviroment throught the bash shell easier and more streamlined some customisation was made to the bash shell prompt
First i created a hidden file called .BashAliasList to add a list of aliases to the bash prompt

#### Alais List added to ".BashAliasList" file
    
    alias pac='sudo pacman'
    alias update='sudo pacman -Syyu'
    alias ls='ls -lar'
    alias e='nvim'
    alias se='sudo nvim'

    This alias file will be quite extensive in the future which is why i made it a seperate file. for this to take effect
    the following line must be appended to the .bashrc file in your home directory "source ~/.BashAlaisList"

### User Directories
while there is a package that can be installed to do this automnaticlly i have opted to setup my user directories manually by creating the following file structure under the home directory
    
    Documents
    Downloads
    Downloads/GitClones
    Music
    Pictures
    Pictures/Wallpapers
    Pictures/Facebook
    Public
    Templates
    videos

### Packages installed

With my shortcuts in bash setup the i can continue setting up a basic working enviroment by installing the following packages
    
    ly (Display/Login Manager) - enabled on startup
    alacritty (terminal emulator)
    hyprland (tiling window manager)
    pipewire & pipewire-pulse (Audio Drivers)
    pulsemixer (terminal based volume control)
    -nvidia (videocard drivers)
    -wofi (application launcher) 
    -git (version control software)
    -google-chrome (browser) - needs to be installed using git
    -ranger (terminal based file manager)
    -hyprpaper (wallpaper utility)

### Hyperland Basic Setup
For changes made to the Hyprland Tiling Window Manager please see the document "Hyprland-ChangeLog.md"
