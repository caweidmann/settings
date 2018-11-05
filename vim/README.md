vim
===

This is a guide for installing a theme for vim across the OS.

## How to install

Make sure that the `256-grayvim.vim` file ends up in the following directory (you’ll need to be root):

    /usr/share/vim/vimXX/colors/ - where XX is the vim version, e.g. 71, 73, or 74

Then open the `vimrc` file so we can add the colour scheme as default for all users:

    vim /usr/share/vim/vimrc

Add the following to the very bottom of the file:

    colorscheme 256-grayvim

Save and exit:

    :wq

Open any file with vim to see the newly added colour scheme.
