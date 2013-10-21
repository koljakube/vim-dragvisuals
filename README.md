# vim-dragvisuals

Drag around visual blocks or lines in vim. Created by Damian Conway, presented at [OSCON 2013](http://www.oscon.com/oscon2013/public/schedule/detail/28875). I simply made the script git-installable and pathogen-compatible.

## Installation

Without [pathogen](https://github.com/tpope/vim-pathogen):

    mkdir -p ~/.vim/plugin
    cd ~/.vim/plugin
    curl -O https://raw.github.com/koljakube/vim-dragvisuals/master/plugin/dragvisuals.vim

As a cloned git repository (with pathogen):

    mkdir -p ~/.vim/bundle
    git clone https://github.com/koljakube/vim-dragvisuals.git ~/.vim/bundle/dragvisuals

Or as a git submodule (also with pathogen):

    mkdir -p ~/.vim/bundle
    git submodule add https://github.com/koljakube/vim-dragvisuals.git ~/.vim/bundle/dragvisuals

After that, add the following to your `.vimrc`, or look into dragvisuals.vim for alternatives:

    vmap  <expr>  <LEFT>   DVB_Drag('left')
    vmap  <expr>  <RIGHT>  DVB_Drag('right')
    vmap  <expr>  <DOWN>   DVB_Drag('down')
    vmap  <expr>  <UP>     DVB_Drag('up')
    vmap  <expr>  D        DVB_Duplicate()

