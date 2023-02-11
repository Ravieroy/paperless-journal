Get more info about fzf [here](https://www.redhat.com/sysadmin/fzf-linux-fuzzy-finder).
fzf is a general-purpose command-line fuzzy finder. In its most basic form, `fzf` works as a filter, processing text from standard input (stdin), then outputting a matching selection to standard output (stdout). In more simpler terms, it takes the input from the output of other programs(for eg. `find` or [[fd]]) and output the matching selection(query). 
### Features 
Some of the cool features are as follows, 
1. Fuzzy finding capabilities allow approximate searches by any part of the match in any order.
2. Super-fast processing speed
3. Interactive match selection lets the user select the desired match after initial filtering.

## Installation 
`fzf` can be installed using [[Package manager]] for specific distribution. For example, 
### Fedora 
```bash 
sudo dnf install fzf
```

### Ubuntu 
```bash 
sudo apt install fzf
```

`fzf` can be installed as plugins in [[Vim]] and [[Neovim]]. For example, using [[vim-plug]], add this line to Vim configuration file : 
```bash
Plug 'junegunn/fzf', { 'do': { -> fzf#install() } }
```

## Upgrading `fzf`
It can be installed like other applications, using [[Package manager]] or depending upon the installation method, this [GitHub Link](https://github.com/junegunn/fzf) has proper instructions to do that. Also read how to [[Install Vim plugins]], if [[vim-plug]] is used to install fzf. 

## Usage 
By default, `fzf` searches all files under the current directory, allows you to filter and search interactively, then prints the result to standard output. `fzf` updates the matches dynamically while we type the search terms in any order.

### Example 1 : Search for file and open in EDITOR 
Suppose we want to search for a file and open it in [[Vim]] for editing, we can use `fzf` to obtain the file name and pass it like this: This will open an interacting panel and we can enter our query and upon selecting the the file, it will open in [[Vim]]
```bash
vim $(fzf)
```

### Example 2 : Search and copy file to destination folder 
Suppose we want to search for a text file and place it in our Templates folder, we can do, 
```bash
cp $(fzf) ~/Templates
```

### Example 3 : Previewing file content
We will be using [[bat]] program to preview the text files on the fly by using the `--preview` command line flag : 
```bash
fzf --preview 'bat --color=always {}'
```

!!! tip
	By default, when we execute `fzf` with no arguments, it uses the `find` command to search for files. For faster and more feature-rich searches, you can replace the default search command with [[fd]] by setting the environment variable `FZF_DEFAULT_COMMAND` like this:
	
	```export FZF_DEFAULT_COMMAND="fd --type f" ```
	
	For permanent changes, set this environment variable in the shell initialization script like `.zshrc` or `.bashrc`.

```bash
export FZF_DEFAULT_OPTS="--height=80% --layout=reverse --info=inline --border --margin=1 --padding=1 --preview 'bat --color=always {}'"
```

```bash
export FZF_DEFAULT_COMMAND="fd --type f"
```

!!! tip
	To enable key bindings, source the corresponding file for the  shell. For example, for Zsh, source `/usr/share/fzf/shell/key-bindings.zsh`: Add this line in the `.zshrc`  file like above to make the changes consistent  across sessions and reboots. Get the file from [here](https://github.com/junegunn/fzf/tree/master/shell) if not found in the above directory.
	
	Once loaded, we can three key bindings for quickly triggering `fzf`
	
	**Ctrl+t**: To select files, similar to autocompletion but with fewer keystrokes
	
	**Alt+c**: To quickly switch into a selected subdirectory
	
	**Ctrl+r**: For smart searching your command history




### Useful Links 
1. [Wiki page of examples](https://github.com/junegunn/fzf/wiki/examples)
2. [Advanced fzf examples](https://github.com/junegunn/fzf/blob/master/ADVANCED.md)
3. [GitHub Link | fzf](https://github.com/junegunn/fzf)
4. [RedHat | fzf](https://www.redhat.com/sysadmin/fzf-linux-fuzzy-finder) 