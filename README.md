bash_aliases
============

This repository stores my all useful bash_aliases


All you need to do is copy this code to .bashrc (or a file you are sourcing from).
(Based on http://stackoverflow.com/a/1423444/2047157 entry)

    if [ -d ~/.bash_aliases ]; then
        for f in ~/.bash_aliases/*.aliases; do . $f; done
    fi

This command will include all files with '.aliases' extension located in .bash_aliases filder in your home.

Then you can create a directory under home and clone this repo.

    git clone https://github.com/Darkless012/bash_aliases.git ~/.bash_aliases
    source ~/.bashrc


# Special dependencies
All aditional dependencies or information, that should be considered are stated below.

## misc.aliases
### timer
This function requires a file to be played as an alarm sound. It would be nice to get one right inside this repo.
Also it uses mplayer.

So far timer plays the file:

    ~/.alarm.ogg


