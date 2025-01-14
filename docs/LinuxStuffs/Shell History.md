It shows the command-line history. The file where history is stored is at `/home/userName/.bash_histiry`. Some common use cases are, 

```bash
Display the commands history list with line numbers:

      history

  Display the last 20 commands (in `zsh` it displays all commands starting from the 20th):

      history 20

  Clear the commands history list (only for current `bash` shell):

      history -c

  Overwrite history file with history of current `bash` shell (often combined with `history -c` to purge history):

      history -w

  Delete the history entry at the specified offset:

      history -d offset
```

1. Run a particular command from the history 
```bash
 ..
 ..
 2775  ls
 2776  pwd
 2777  hostname
 ..
 ..
```

Now simply open the [[Terminal]] and type the line number with `!` in front of it,
```bash
# This will run the hostname command.
!2777
```

2. Search for a keyword inside the history 
```bash
history | grep query
```

