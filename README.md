# Configurations for zsh and oh-my-zsh

1. Install zsh and git and change to zsh

```
sudo apt install git zsh
```

2. Install [oh my zsh](https://ohmyz.sh/#install)

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

3. Copy theme xiong-chiamiov-custom.zsh-theme to themes folder

```
cp xiong-chiamiov-custom.zsh-theme ~/.oh-my-zsh/themes/
```

4. Edit .zshrc and set xiong-chiamiov-custom as your theme

```
ZSH_THEME="xiong-chiamiov-custom"
```

5. Install plugins: [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) and [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

```

6. Edit .zshrc and set plugins
```
plugins=(
git
zsh-autosuggestions
zsh-syntax-highlighting
)
```

7. Refresh configuration file

```
source .zshrc
```