zsh prompt config and functions to use with rvm or git.

# Install with oh-my-zsh

    git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
    mv ~/.zshrc ~/.zshrc.orig
    cp -i ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc

# Install zsh-prompt

    git clone git://github.com/dmitrynix/zsh-prompt.git ~/.zsh-prompt

# Configure

Append to zsh config file:

    # Customize to your needs...
    [[ -s $HOME/.rvm/scripts/rvm ]] && source $HOME/.rvm/scripts/rvm
    source ~/.zsh-prompt/load

    PROMPT=$'%1d$(prompt_git_info)%# '
    RPROMPT='$(rvm_ruby_prompt)'

