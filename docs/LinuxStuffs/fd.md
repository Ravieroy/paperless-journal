# fd 
**fd** is a simple, fast, and user-friendly tool meant to simply perform faster compared to **find**. It is not meant to completely replace **find**, but rather give you an easy-to-use alternative that performs slightly faster.

## Installation 
`fd` can be installed for different Linux distributions using the default package manager, for example, 

### Debian/Ubuntu based distros
```bash
sudo apt install fd-find
```

### Fedora (RHEL)
```bash
sudo dnf install fd-find
```

### Arch based distros
```bash
sudo pacman -S fd
```

## Usage 
- The simplest usage is to feed the query as arument to `fd`
```bash
fd <query> # syntax
fd config # example 
```

- Let’s say we want to find all jpg files. We can use the `-e` flag to filter by file extension:
```bash
fd -e jpg
```

- If we want to exclude some results, you can use the `-E` flag like this:
```bash
fd -e pdf -E miniconda3
```
This command will look for all files with pdf extension, and will exclude results from the **miniconda3** directory.

- If we want to specify a search directory, we simply need to give it as an argument:
```bash
fd <pattern> <directory>
```

- We can use `-x` or `--exec` arguments to perform parallel command execution with the search results.
```bash
fd -e txt -x chmod 644 {}
```

For more visit [fd | Tecmint](https://www.tecmint.com/fd-alternative-to-find-command/).

