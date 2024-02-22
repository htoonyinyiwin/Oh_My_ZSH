# Guide to install Oh_My_ZSH the simplest way

Simply execute the below single command

```sh
bash -c "$(curl -fsSL https://raw.githubusercontent.com/htoonyinyiwin/Oh_My_ZSH/main/setup.sh)"
```
Or the following one command after another for better understanding

```sh
sudo apt update
```
Install zsh shell:
```sh
sudo apt install zsh
```
Install font-powerline
```sh
sudo apt-get install fonts-powerline
```
Change default shell into zsh
```sh
chsh -s /usr/bin/zsh
```

#install ohmyzsh using curl

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```sh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
```sh
sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc
```

#Or edit inside .zshrc file > ZSH_THEME="powerlevel10k/powerlevel10k"

```sh
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```
```sh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```
```sh
sed -i 's/plugins=(git)/plugins=(git zsh-autosuggestions zsh-syntax-highlighting)/' ~/.zshrc
```

#Or edit inside .zshrc file > plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

```sh
source ~/.zshrc
```
