git clone git@github.com:miukoba/dotfiles-mac.git

ln -s ~/dotfiles-mac/gitconfig ~/.gitconfig

ln -s ~/dotfiles-mac/gitignore ~/.gitignore

vi ~/.zshrc

```
alias g='git'

# with zim
alias ggpull='git pull origin "$(git-branch-current)"'
alias ggpush='git push origin "$(git-branch-current)"'

# history
HISTSIZE=1000000
SAVEHIST=1000000

# mcfly
eval "$(mcfly init zsh)"
```
