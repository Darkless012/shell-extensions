bash_aliases
============

This repository stores my all useful bash_aliases


All you need to do is copy this code to .bashrc (or a file you are sourcing from).

    if [ -d ~/.bash_aliases ]; then
        . ~/.bash_aliases/*.aliases
    fi

This command will include all files with '.aliases' extension located in .bash_aliases filder in your home.

Then you can create a directory under home and clone this repo.

    mkdir ~/.bash_aliases
    cd ~/.bash_aliases
    git clone https://github.com/Darkless012/bash_aliases.git
    source ~/.bashrc