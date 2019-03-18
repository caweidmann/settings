Terminal
========

#### Add VS Code to terminal

https://code.visualstudio.com/docs/setup/mac

#### Install homebrew

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

#### Install oh my zsh

    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#### Install auto suggestions

From https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md, boils down to:

    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

    code ~/.zshrc
    
    # Add the following line 
    plugins=(zsh-autosuggestions)

#### Install custom theme

    # Install fonts for theme
    git clone https://github.com/powerline/fonts.git
    cd fonts
    ./install.sh
    
    # Change the theme
    code ~/.zshrc
    ZSH_THEME="agnoster"

https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38

_"Tango Dark" preset. Cursor hex = a9e8e8. Foreground hex = 7eb1b1._

#### Remove user name:

    code ~/.zshrc

    # Add the following line
    DEFAULT_USER=$USER

### _Other_

Show git branches inline:

    git config --global pager.branch 'false'

Create SSH key:

    ssh-keygen -t rsa -C "your_email@example.com"

Copy SSH key:

    pbcopy < ~/.ssh/id_rsa.pub
    
Things to configure/remember:
- Allow unlimited scroll back lines


### _For Windows with WSL:_

https://github.com/lloydstubber/my-wsl-setup

https://medium.com/@ssharizal/hyper-js-oh-my-zsh-as-ubuntu-on-windows-wsl-terminal-8bf577cdbd97

Change auto suggestsion colour manaully in ~/.zshrc:

    ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=5'

Only fonts that worked for me were:
- DejaVu Sans Mono for Powerline
- Droid Sans Mono Dotted for Powerline
- Droid Sans Mono Slashed for Powerline
- Go Mono for Powerline
