# New Mac Web Dev Setup scripts

## Pre-Setup
Install homebrew and git, and set up SSH for Github
```
curl --remote-name https://raw.githubusercontent.com/colbycheeze/dotfiles/master/setup/pre-setup.sh
less mac
sh mac 2>&1 | tee ~/laptop.log
```
Install latest (non beta) Xcode from the [app store](https://developer.apple.com/xcode/downloads/)

## Setup
   `git clone git@github.com:colbycheeze/dotfiles.git ~/dotfiles && cd ~/dotfiles && chmod a+x setup.sh && ./setup/setup.sh`

## Finishing touches
  1. Register Divvy and add any hotkeys for window management
  1. Change key repeat rate with karabiner (delay: 225, repeat: 25)
  1. Swap ESC and CAPS key with seil: [(instructions)](http://stackoverflow.com/a/8437594)
  1. Connect iterm2 profile to dotfiles: [(instructions)](http://stackoverflow.com/a/25122646/4298624)
  1. open `nvim` and run `:PlugInstall` and `:UpdateRemotePlugins`

## Customizing
I certainly do NOT recommend installing all of my setup without looking through what is happening and customizing it for yourself. Fork this repo and update anything you like.

Look through the shell scripts  in `setup` folder to see what programs are being installed. You can add or remove everything from there. Most likely, if you are not a VIM power user you will want to modify some of the atom plugins and config to suit yourself.
