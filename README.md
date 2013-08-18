# zsh-comp-gsettings
It is a zsh completion script for gsettings.
It takes advantage of compsys functions of zsh.

## How to Use
It can be automatically loaded when you login or run zsh.

1. Copy the script named _gsettings into any one of your fpath directories.
2. Restart zsh

You can see where are your fpath directories by running `echo $fpath`.If every fpath direcotory is system one and you want to install the script into your personal directory, you can do that. Copy the script into your personal directory, and add the direcotry into the fpath in your ~/.zshrc. That has to be done before calling compinit. For your information, perhaps that part of your .zshrc will look like the following:

```
typeset -U fpath
fpath=($fpath $your_directory)
autoload -Uz compinit
compinit
```

## Completion to be More Complete
You can help me improve the gsettings completion. If you find any problems or you have other preferences for completion style, feel free to file your issues. Any patch is welcome.

## Tested Version
* gsettings: 2.36
* zsh: 5.0.2

## About gsettings
[Spec of gsettings command](https://developer.gnome.org/gio/2.36/gsettings-tool.html)
