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

4. You can use a theme of oh-my-zsh or use my custom theme in folder in oh-my-zsh-theme (copy the theme to ~/.oh-my-zsh/themes), after that edit .zshrc and set your selected theme.

```
ZSH_THEME="xiong-chiamiov-custom"
```

- Alternatively you can install [starship](https://starship.rs/guide/#%F0%9F%9A%80-installation) and customize your theme as you prefer, in the .zshrc you have to set:

```
ZSH_THEME=""
```

- Set your configuration of starship in ~/.config/starship.toml (or use my configuration in starship-configuration/starship.toml).

- Important, it's neccesary install [Nerd Fonts](https://www.nerdfonts.com/) for showing icons in your terminal.


5. Install plugins: [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) and [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

6. Edit .zshrc and set plugins
```
plugins=(
git
zsh-autosuggestions
zsh-syntax-highlighting
history-substring-search
)
```

7. Refresh configuration file

```
source .zshrc
```
