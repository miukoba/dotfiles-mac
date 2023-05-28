git clone git@github.com:miukoba/dotfiles-mac.git

ln -s ~/dotfiles-mac/gitconfig ~/.gitconfig

ln -s ~/dotfiles-mac/gitignore ~/.gitignore

vi ~/.zshrc

```
alias g='git'
export EDITOR=vim

alias ggpull='git pull origin "$(git-branch-current)"'
alias ggpush='git push origin "$(git-branch-current)"'

# history
HISTSIZE=1000000
SAVEHIST=1000000
setopt HIST_EXPIRE_DUPS_FIRST
setopt HIST_IGNORE_DUPS
setopt HIST_IGNORE_ALL_DUPS
setopt HIST_FIND_NO_DUPS
setopt HIST_SAVE_NO_DUPS

