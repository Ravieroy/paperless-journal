`nnn` is a full-featured terminal file manager. It's tiny, nearly zero-config and incredibly fast. For more detail information see project's [GitHub Link](https://github.com/jarun/nnn).

## Installation 
### Ubuntu 
```bash
sudo apt install nnn
```

### Fedora 
```bash
sudo dnf install nnn
```

There is no config file. Associated files are at, 
```bash
${XDG_CONFIG_HOME:-$HOME/.config}/nnn/
```

`nnn` doesn't have config file and instead it uses environmental variables which can be set in shell config file as follows,(See [usage](https://github.com/jarun/nnn/wiki/Usage) to see what the following does.)
```bash
export NNN_BMS='h:~;p:~/Pictures;d:~/Downloads;m:~/my-stuffs;s:~/.scripts;c:~/.config;b:bookmarks'
export NNN_COLORS='1234'
export NNN_PLUG='x:!chmod +x $nnn'
```

