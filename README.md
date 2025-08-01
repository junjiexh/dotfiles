# Setup

```
# 1. Create the alias first (needed for the checkout)
alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

# 2. Add alias to shell config for persistence
echo "alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> ~/.zshrc

# 3. Clone the bare repository
git clone --bare https://github.com/junjiexh/dotfiles.git $HOME/.dotfiles

# 4. Checkout the files to your home directory
dotfiles checkout
```

set up p10k:
need to install oh-my-zsh in advance
```
echo '[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh' >> ~/.zshrc
```
