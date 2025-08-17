# Working Enviroment
This "WorkingEnviroment" branch has been created to serve the folling purposes.
+ Create a useable working enviroment within the TTY Bash Shell after logging into a fresh installation of Arch Linux
+ Create a Bash Shell Script that can be executed to deploy my custom usable working enviroment on a fresh installation of Arch Linux.

## Creating a Usable Working Enviroment
After rebooting the system and logging into a fresh installation of Arch Linux a usable working enviroment for use in the TTY would be helpful. 
> Note: All development on the "WorkingEnviroment" branch of this projects repository s done on a fresh install of Arch Linux this means all file,scripts and configurations are designed to be rn on a fresh install of Arch Linux.*

## Creating the WorkingEnviroment Shell Script
A Bash Shell Script file has been created name "WorkingEnviroment.sh" with the purpose of when executed it will deploy the final useable working enviroment on any fresh installtion of Arch Linux.
> Note: For further information please see the contents of the "WorkingEnviroment-ToDoList.md" for a current list of tasks regarding the "WorkingEnviroment.sh" bash shell script. Alternativly you can view the contents of the shell scripts itself as it is heavyly documented. 

## Setting up a working Bash Enviroment
To make for more a efficient use some modification to the bash shell enviroment have been made.

### Bash Aliases
As there is the possiability of the list of personally used alias commands growing quite large a hidden file name ".BashAliases" has been createdi with the follow aliases and potential of further segmentation of alias files
    
    alias ls='ls -lar' # Appends ls command to show all files in long format with human readable file size
    alias ..='cd ..' # Shortcut for go up one directory
    alias ...='cd ../..' # Shortcut for go up two directories

    alias pac='sudo pacman' # Alais for calling pacman with superuser
    alias update='sudo pacman -Syyu' # Fully sync and update packages with pacman
    alias vim='nvim' # Replaces vim command with neovim command
    alias vi='nvim' # Replace vi command with neo vim comm

A section regarding the Bash Aliases has been added to the "WorkingEnviroment.sh" bash shell script. 

## Setting up User Directories
There is a package that can be install via pacman and do this for you however i have decided to setup my user directories manually for now using the following user directory structure.
    
    Documents
    Downloads
    Downloads/GitClones
    Music
    Pictures
    Pictures/Wallpapers
    Projects
    Public
    Templates
    Videos

A section regarding creation of user directories has been added to the "WorkingEnviroment.sh" bash shell script

## Setting up a Working Git Enviroment
A working Git Enviroment is required be setup on the system along with the following git variables set.

    global.name # Sets the global name for git
    global.email # Sets the global email for git
    Personal Access Tokens # All Personal Access Tokens will be managed seperatly.

A section regarding the setting up of a working git enviroment has been added to the "WorkingEnviroment.sh" bash shell script
