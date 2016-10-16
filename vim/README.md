vim
===

256-grayvim.vim = Can be downloaded and put into correct directory.  

## How to

Make sure that the `256-grayvim.vim` file ends up in the following directory (you’ll need to be root):

    /usr/share/vim/vimXX/colors/ -  where XX is the vim version, e.g. 71, 73, or 74

Then add the colorscheme as default for all users:

    vim /usr/share/vim/vimrc

Add the following to the very bottom of the file:

    colorscheme 256-grayvim

Save and exit. Next time you open any file with vim the colour scheme should be applied.
