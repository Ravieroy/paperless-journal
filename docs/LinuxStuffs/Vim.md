# Vim
It is a contraction of Vi Improved, and a [[FOSS]], screen-based text editor authored by , Bram Moolenaar. It is an improved clone of Bill Joy's `vi`. [[Neovim]] is another fork of Vim that improves the extensibility and maintainability of Vim. 

Users who are just getting started, the [[Vim and Neovim]] is not that apparent and are basically identical. 

## Installation 
`vi` is usually pre-installed in most [[Linux distros]] but `vim` needs to be mannualy installed using respective [[Package Manager]] of the distro. For Ubuntu/Debian based distros, 
```bash
sudo apt install vim
```
## Usage 
Inorder to start vim, one can simply type `vim` in [[Terminal]] and start using it. To open any file in vim one can use
```bash
vim fileName 
```

## Useful Commands (Brief)
`vim` has some common modes . The most important modes are:

- **Normal mode** – used for editor commands. This is also the default mode, unless the insertmode option is specified.
- **Visual mode** – similar to normal mode, but used to highlight areas of text. Normal commands can be run on the highlighted area, for instance to move or edit a selection.
- **Insert mode** – similar to editing in most modern editors. In this mode, buffers can be modified with the text inserted.
- **Command-line or Cmdline mode** – supports a single line input at the bottom of the Vim window. Normal commands (beginning with :), and some other keys for specific actions (including pattern search and the filter command) activate this mode. On completion of the command, Vim returns to the previous mode.

`i` : Insert mode (To start editing)
*esc* : Press esc button to enter in Command mode
`:w` : Save the file but continue editing
`:wq` : Save and exit
`:q` : Exit without saving
`:q!` : Ignore the changes made and exit

For more commands and shortcuts read [[Useful Vim Commands]]. 







