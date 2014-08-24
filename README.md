Open Guake terminal here
========================

A Nautilus Python extension adding a entry in the right click menu to open the Guake terminal in the current directory.

When clicked, Guake gets the focus, creates a new tab and sets the current directory to the directory you where in Nautilus.

This is a fork from [ksamuel's script](https://github.com/ksamuel/Open-guake-here), updated with the following changes:
* Auto name new Guake tab, according to the last directory in the path. For example if you open '/abc/def/ghi', the new tab wil be named 'ghi'.
* Fix handling of special directories like Desktop or Trash
* Fix new tab not getting focus in Ubuntu 14.04

GPLv2 licence. Enjoy.


## How to install

On Ubuntu:

    sudo apt-get install python-nautilus curl
    mkdir -p ~/.local/share/nautilus-python/extensions
    curl -L https://raw.githubusercontent.com/desbma/Open-guake-here/master/open-guake-terminal.py > ~/.local/share/nautilus-python/extensions/open-guake-terminal.py
    chmod +x ~/.local/share/nautilus-python/extensions/open-guake-terminal.py


### If Nautilus is not in English language

In this case you may need to replace `~/Desktop` in the script by the name of your Desktop directory (for example in French it's `~/Bureau`).
