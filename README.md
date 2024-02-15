git clone git@github.com:miukoba/dotfiles-mac.git

ln -s ~/dotfiles-mac/gitconfig ~/.gitconfig

ln -s ~/dotfiles-mac/gitignore ~/.gitignore

ln -s ~/dotfiles-mac/starship.toml ~/.config/starship.toml

vi ~/.zshrc

```

alias g='git'
alias fullpath="readlink -f"

export EDITOR=vim
export PATH=$HOME/bin:$PATH

alias ggpull='git pull origin "$(git-branch-current)"'
alias ggpush='git push origin "$(git-branch-current)"'

# history
HISTSIZE=1000000
SAVEHIST=1000000
setopt share_history           # 履歴を他のシェルとリアルタイム共有する
setopt hist_ignore_all_dups    # 同じコマンドをhistoryに残さない
setopt hist_ignore_space       # historyに保存するときに余分なスペースを削除する
setopt hist_reduce_blanks      # historyに保存するときに余分なスペースを削除する
setopt hist_save_no_dups       # 重複するコマンドが保存されるとき、古い方を削除する
setopt inc_append_history      # 実行時に履歴をファイルに追加していく
