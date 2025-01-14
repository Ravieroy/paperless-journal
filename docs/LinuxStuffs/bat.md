Links : [Releases](https://github.com/sharkdp/bat/releases), [GitHub](https://github.com/sharkdp/bat)

## Functionality 
A `cat` clone with syntax highlighting and Git integration. 

## Installation 
*RECOMMENDED*
Get the `.deb` file from the [release](https://github.com/sharkdp/bat/releases) page.
```bash
sudo dpkg -i bat_0.18.3_amd64.deb  # adapt version number and architecture
```

*FROM APT REPOSITORY*
```bash
sudo apt install bat
```

***If you install `bat` this way, please note that the executable may be installed as `batcat` instead of `bat` (due to [a name clash with another package](https://github.com/sharkdp/bat/issues/982)). You can set up a `bat -> batcat` symlink or alias to prevent any issues that may come up because of this and to be consistent with other distributions:***

```bash
mkdir -p ~/.local/bin
ln -s /usr/bin/batcat ~/.local/bin/bat
```

## Usage
```bash
bat fileName
```
***An alias `alias cat="bat"` can be added in the *.bashrc* file to keep using `cat` but with the functionality of `bat`. After adding the alias,***

```bash
source .bashrc
```
*There are other [[Terminal]] shells like [[zsh]] and others. All of them have a file similar to .bashrc*

----
Useful Links :
1. [[Set An Alias]]



