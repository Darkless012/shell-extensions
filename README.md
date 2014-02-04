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