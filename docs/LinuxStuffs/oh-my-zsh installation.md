## Oh-my-zsh Installation
---
***Dependencies***
1. curl
2. git

**Step 0: Install [[zsh]] shell**
For this plugin to work, we need [[zsh]] shell to be installed in the system. Use the following command,
```bash
sudo apt install zsh
```

**Step 1: Install Oh-My-Zsh using Curl :**
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

**Step 2: Install zsh-autosuggestions by running:**
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

**Step 3: Install zsh-syntax-highlighting by running:**
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

**Step 4: Use your preferred text editor. Here [[Vim]] is used**
```bash
vim .zshrc
```
Search for plugins section in the `.zshrc` file and replace the line with the following,
*plugins=(git zsh-autosuggestions zsh-syntax-highlighting)*

***Change zsh Theme***

By default the `robbyrussel` is installed. It can be changed to any other theme by replacing the `robbyrussel` to `agnoster`
```bash
ZSH_THEME="agnoster"
```
*See [[Fonts installation]] to fix weird glyphs appearing in terminal in this theme*

***Make zsh default shell***

Use the following command in [[Terminal]] to make `zsh` your default shell.
```bash
chsh -s $(which zsh)
```
*The effect we take into effect after reboot*
