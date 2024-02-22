# Guide to install Oh_My_ZSH the simplest way

```sh
sudo apt update
```
sudo apt install zsh

sudo apt-get install fonts-powerline

chsh -s /usr/bin/zsh

#install ohmyzsh using curl

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc

#Or edit inside .zshrc file > ZSH_THEME="powerlevel10k/powerlevel10k"

git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

sed -i 's/plugins=(git)/plugins=(git zsh-autosuggestions zsh-syntax-highlighting)/' ~/.zshrc

#Or edit inside .zshrc file > plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

source .zshrc
