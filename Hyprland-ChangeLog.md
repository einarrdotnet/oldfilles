# Arch Linux Post Install Hyprland Change Log

Due to the extensive amount of changes being made to the Hyprland Tiling Window Manager this document was created as a extension of the Main-ChangeLog.md.
This file serves to document all changes made speficilly to the Hyperland Window Manger after a fresh install of the package.

## Copying Default Configuration Files
Before logging into Hyprland a copy of the default cofiguration files must be made
    create directory in home folder named ".config" if it already does not exsist
    copy the directory and its contents /usr/share/hypr to the new .config file in the home directory
a backup of the default configuration files should also be made
    in the new .config/hypr directory make a backup of the hyprland.conf file name it hyprland.conf.bak


##Getting Things Functional
in order to make hyprland somewhat function the following edits to the hyprland.conf file was made
these edit are required to be made before logging in first time
    -changed $terminal vairable to use alacritty instead of kitty
    -Changed Keybinding to open a terminal to "bind = $mainMod, Return, exec, $terminal"
    -Changed Keybinding to close active window to "bind = $mainMod, q, killactive"
    -Changed Keybind to exit Hyprland to "bind = CTRL ALT, Delete, Exit"
