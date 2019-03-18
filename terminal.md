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
    cd ..
    rm -rf fonts

    # Change the theme
    code ~/.zshrc
    ZSH_THEME="agnoster"

    # Change colours
    1. Open iTerm2 > Preferences > Profiles > Colors
    2. Under "Color Presets" select "Tango Dark"
    3. Cursor hex = a9e8e8
    4. Foreground hex = c5e7e7

    # Change font
    1. Open iTerm2 > Preferences > Profiles > Text > Change Font
    2. Select "Meslo LG S for Powerline" font
    
    # Change background image
    1. Open iTerm2 > Preferences > Profiles > Window
    2. Select current Desktop background from Library > Desktop Pictures > El Capitan 2
    3. Reduce blending
    
    # Unlimited scrollback
    1. Open iTerm2 > Preferences > Profiles > Terminal
    1. Select checkbox "Unlimited scrollback"

https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38

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
