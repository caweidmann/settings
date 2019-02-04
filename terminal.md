Terminal
========

Install oh my zsh:

    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Install auto suggestions:

https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md

To install custom theme:

https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38

Remove user name:

    code ~./zshrc
    # Add the following line to the rc file:
    DEFAULT_USER=$USER

Create SSH key:

    ssh-keygen -t rsa -C "your_email@example.com"
    
Things to remember:
- Allow unlimited scroll back lines
