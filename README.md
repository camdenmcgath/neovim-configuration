# neovim-configuration
Configuration files for settings and plugins used in my Neovim setup

## Platform support
So far this configuration has only been used on Ubuntu18.04 on Windows Subsystem for Linux 2 in the Windows terminal.
Support and testing in other environments such as Windows, native Linux, and other versions of Ubuntu on WSL2 will be coming once
this configuration is more functional and complete.

## Pre-Requisites
#### Must have Neovim installed. 
This is how I installed it from source on Ubuntu18.04 WSL2:
```
sudo apt-get install ninja-build gettext libtool libtool-bin autoconf automake cmake g++ pkg-config unzip curl doxygen
git clone https://github.com/neovim/neovim
cd neovim && make CMAKE_BUILD_TYPE=RelWithDebInfo
sudo make install (installs to /usr/local)
```
#### Install Packer for managing plugins:
```
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install packer
```
#### Create config file structure:
If not created during installation of nvim, create a ~/.config/nvim directory to store my cloned configuration files. 

## Installing my Configuration !!
#### Cloning
Run 
