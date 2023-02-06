# Command Line Utility: *lsd*
Links : [GitHub](https://github.com/Peltoche/lsd), [Releases](https://github.com/Peltoche/lsd/releases)

---

## Functionality:
`lsd` is a command line utility which can be used instead of `ls`. It is a rewrite of GNU `ls` with a lot ofadded features like colors, icons, tree-view, more formatting options etc.

## Installation 
For Ubuntu based distros,use the deb package which you can download from the  [release page](https://github.com/Peltoche/lsd/releases). Once the deb file is downloaded, head over to the directory and install by following command, 

```bash
sudo dpkg -i lsd_0.21.0_amd64.deb
```
*use the correct name in above command*

## Usage
Once installed successfully,it can be used just like `ls` command. Instead of `ls` now use `lsd`

***Some kind of font packages like [Font Awesome](https://fontawesome.com/) or [Nerd Fonts](https://www.nerdfonts.com/) are required for this to work nicely. [[Fonts installation]] is quite easy on Linux as well.*** 

***An alias `alias ls="lsd"` can be added in the .bashrc file to keep using `ls` but with the functionality of `lsd`. After adding the alias,***

```bash
source .bashrc
```
*There are other [[Terminal]] shells like [[zsh]] and others. All of them have a file similar to .bashrc *

***Known Issue***

`lsd` has been known to have issues with displaying folders which has root access. Sometimes it just doesn't work. This could happen when the `snap` version is installed. `lsd` just doesn't have the right file permissions in those cases. The best way is to use the deb package to install.
[Link](https://github.com/Peltoche/lsd/issues/79)
