Aliases are user defined custom commands which can save lot of our time typing long commands. List of defined aliases on profile can be checked by simply executing the following command in [[Terminal]]
```bash
alias
```

## Creating permanent aliases 
To keep **aliases** active between sessions, we can save them in our user’s shell configuration profile file. This can be, 
- Bash : `~/.bashrc`
- Zsh : `~/.zshrc`

Open the config file for the shell in [[Vim]] by executing, 
```bash
vim .zshrc
```

Suppose we frequently edit our i3 config file and want to set an alias for it, we can put the following line in our config file, 
```bash 
alias i3edit="vim ~/.config/i3/config"
```

One can use one's preffered text editor in place of vim in the above command. Next we simply source the config file for the change to take effect. 
```bash
source .zshrc
```

### Creating User or Global Alias

To create a user alias, simply make the changes in the `/home/user/.bashrc` file while for any global alias make the changes in `/etc/bashrc` file. 
