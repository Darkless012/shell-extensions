This repository stores my all useful shell aliases and other functions.
Because I've started to use fish as a default shell, I've preserved all bash related stuff into *bash* folder.

# fish

## Installation

### clone

    git clone https://github.com/Darkless012/shell-extensions.git ~/.shell-extensions

### modify config.fish

Add this code to .config/fish/config.fish

```
if test -d ~/.shell-extensions
    for f in ~/.shell-extensions/fish/*.aliases
        . $f
    end
end
```

### source

Then you can source the .bashrc and all aliases should work.

    source ~/.config/fish/config.fish

# bash

## Installation

### clone

    git clone https://github.com/Darkless012/shell-extensions.git ~/.shell-extensions

### modify .bashrc

Add this code to .bashrc (or a file you are sourcing from).
(Based on http://stackoverflow.com/a/1423444/2047157 entry)

```
    if [ -d ~/.shell-extensions/bash ]; then
        for f in ~/.shell-extensions/bash/*.aliases; do . $f; done
    fi
```

This command will include all files with '.aliases' extension located in bash sub-folder.

### source

Then you can source the .bashrc and all aliases should work.

    source ~/.bashrc

## Special notes

### Private aliases
After cloning this repository, you want to have some private (not publicly shared) aliases.
For this purpose you can create/use *private.aliases* file which is .gitignore(d)

### misc.aliases - timer
This function requires a file to be played as an alarm sound. It would be nice to get one right inside this repo.

Also it uses mplayer (you need to have it installed).

So far timer plays the file, which you need to create/obtain by yourself:

    ~/.alarm.ogg
