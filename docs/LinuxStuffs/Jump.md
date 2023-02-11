
Jump gives quick access to the most visited directory for the shortest search term we type. 

## Installation 
The *deb* and *rpm* package for Ubuntu and Fedora respectively can be downloaded from the [releases](https://github.com/gsamokovarov/jump/releases) section of the [jump Github repository](https://github.com/gsamokovarov/jump). The following commands can also be used to directly download and install the program.

### Debian/Ubuntu 
```bash
wget https://github.com/gsamokovarov/jump/releases/download/v0.51.0/jump_0.51.0_amd64.deb && sudo dpkg -i jump_0.51.0_amd64.deb
```

### Fedora
```bash
wget https://github.com/gsamokovarov/jump/releases/download/v0.51.0/jump_0.51.0_amd64.deb && sudo dpkg -i jump_0.51.0_amd64.deb
```

## Integrate jump with shell
Add the following line in `~/.bashrc`, `~/bash_profile` or `~/.zshrc`  :
```bash
eval "$(jump shell zsh)"
```

## Usage 
The usefullness of `j` is seen after it has build database of the frequently visited directories. Suppose we go into the config file of polybar using normal way of `cd`
```bash 
cd ~/.config/polybar
```
Then, from anywhere else, we can go to the directory polybar by simply typing, 
```bash 
j pol
```

For more use cases, visit [GitHub Link](https://github.com/gsamokovarov/jump). 




