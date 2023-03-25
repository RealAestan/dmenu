# Custom build of dmenu v5.2

This build uses:
- border (`-bw`)
- center (`-c`)
- password (`-P`)
- xresources (dmenu.font, dmenu.background, dmenu.foreground, dmenu.selbackground, dmenu.selforeground)
- fuzzymatch (`-F` to disable it)
- fuzzyhighlight with xresources compat (dmenu.hibackground, dmenu.hiforeground, dmenu.selhibackground, dmenu.selhiforeground)
- lineheight (`-h`)
- rejectnomatch (use `-r` and disable fuzzymatch if you want to use it)
- emoji support (see allow-color-font patch)

## Requirements
In order to build dmenu you need the Xlib header files.


## Installation

Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


## Running dmenu

See the man page for details.
