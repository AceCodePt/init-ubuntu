# regular update
sudo apt-get update

# Better terminal
sudo apt install zsh

# basic stuff
sudo apt-get install ripgrep
sudo apt install curl
sudo apt install fzf

# install neovim
sudo snap install nvim --classic

# install clipboard tool
sudo apt-get install xclip

# swap capslock and escape
echo 'setxkbmap -option caps:swapescape' >> ~/.profile

# pretty esenital stuff
sudo apt install git
sudo apt install build-essential libssl-dev

# install rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# node version manager
SHELL=/bin/zsh
curl -fsSL https://fnm.vercel.app/install | bash

# lazy git
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": "v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/latest/download/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit /usr/local/bin
rm -rf lazygit
rm -rf lazygit.tar.gz

fnm install 18 

LV_BRANCH='release-1.3/neovim-0.9' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh)

# Install font
https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/Hack.zip


