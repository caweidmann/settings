Terminal
========

### _For Windows with WSL:_

Install zsh:

    sudo apt-get install zsh

Then follow steps for Mac below.

### _For Mac_

#### Install oh my zsh

    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#### Install auto suggestions

    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

Add the plugin to plugins list:

    code ~./zshrc
    
Add the following line to the rc file:

    plugins=(zsh-autosuggestions)

https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md

#### Install custom theme

https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38

_"Tango Dark" preset. Cursor hex = a9e8e8. Foreground hex = 7eb1b1._

#### Remove user name:

    code ~./zshrc

Add the following line to the rc file:

    DEFAULT_USER=$USER

### _Other_

Create SSH key:

    ssh-keygen -t rsa -C "your_email@example.com"

Copy SSH key:

    pbcopy < ~/.ssh/id_rsa.pub
    
Things to configure/remember:
- Allow unlimited scroll back lines
