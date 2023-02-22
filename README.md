# My_Mac_Setting

## Install iTerm2
```
brew install --cask iterm2
```

## Install Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install PowerLevel10K Theme for Oh My Zsh
```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
Now that it's installed, open the "~/.zshrc" file with your preferred editor and change the value of "ZSH_THEME" as shown below:
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
To reflect this change on your terminal, restart it or run this command:
```
source ~/.zshrc
```

## Install Meslo Nerd Font

## Update VSCode Terminal Font
Open settings.json and add this line:
```
"terminal.integrated.fontFamily": "MesloLGS NF"
```

## Configure PowerLevel10K
Restart iTerm2. You should now be seeing the PowerLevel10K configuration process. If you don't, run the following:
```
p10k configure
```

## Change iTerm2 Colors to My Custom Theme
1. Open iTerm2
2. Open iTerm2 preferences
3. Go to Profiles > Colors
4. Import the downloaded color profile (japanesque)
5. Select the color profile (japanesque)
You can download japanesque here:
https://github.com/aereal/dotfiles/tree/main/colors/Japanesque


## Install ZSH Plugins
Install zsh-autosuggestions:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
Install zsh-syntax-highlighting:
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
Open the "~/.zshrc" file in your desired editor and modify the plugins line to what you see below.
```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```
Load these new plugins by running:

# You're Done!
To make this setting, I refer to below pages.


# references
1. https://www.josean.com/posts/terminal-setup
2. https://this.aereal.org/entry/2016/03/22/120000
