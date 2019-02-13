Terminal
========

### _For Windows with WSL:_

https://github.com/lloydstubber/my-wsl-setup#fix-the-ls-and-cd-colours

https://medium.com/@ssharizal/hyper-js-oh-my-zsh-as-ubuntu-on-windows-wsl-terminal-8bf577cdbd97

Change auto suggestsion colour manaully in ~/.zshrc:

    ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=5'

### _For Mac_

#### Install oh my zsh

    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#### Install auto suggestions

From https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md, boils down to:

    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

    vim ~./zshrc
    
    # Add the following line 
    plugins=(zsh-autosuggestions)

#### Install custom theme

https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38

_"Tango Dark" preset. Cursor hex = a9e8e8. Foreground hex = 7eb1b1._

#### Remove user name:

    vim ~./zshrc

    # Add the following line
    DEFAULT_USER=$USER

### _Other_

Create SSH key:

    ssh-keygen -t rsa -C "your_email@example.com"

Copy SSH key:

    pbcopy < ~/.ssh/id_rsa.pub
    
Things to configure/remember:
- Allow unlimited scroll back lines
