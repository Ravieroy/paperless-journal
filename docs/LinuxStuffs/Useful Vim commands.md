| KEYBINDING |     | ACTION               |
| ---------- | --- | -------------------- |
| :q         |     | Close File           |
| :qa        |     | Close all Files      |
| :w         |     | Save                 |
| :wq / :x   |     | Save and Close Files |
| ZZ         |     | Save and Quit        |
|            |     |                      |

## Navigation
| KEYBINDING        |     | ACTION                           |
| ----------------- | --- | -------------------------------- |
| `h` `j` `k` `l`           |     | Arrow Keys                       |
| ==WORD==          |     |                                  |
| `<C-B>` / `<C-F>` |     | Page up/down                     |
| b /w              |     | Previous/next word               |
| ge / e            |     | Previous/Next Word               |
| ==LINE==          |     |                                  |
| 0                 |     | Start of line                    |
| ^                 |     | Start of line(after workspace)   |
| $                 |     | End of line                      |
| ==CHARACTER==     |     |                                  |
| fc                |     | Go forward to character c        |
| Fc                |     | Go backward to character c       |
| ==DOCUMENT==      |     |                                  |
| gg                |     | First Line                       |
| G                 |     | Last Line                        |
| :{number}         |     | Go to line {number}              |
| {number}G         |     | Go to line {number}              |
| {number}j         |     | Go down {number} lines           |
| {number}k         |     | Go down {number} lines           |
| ==SEARCH==        |     |                                  |
| /                 |     | Trigger search in normal mode    |
| n                 |     | Next matching search pattern     |
| N                 |     | Previous match                   |
| *                 |     | Next whole word under cursor     |
| #                 |     | Previous whole word under cursor |
| ==TAB PAGES==     |     |                                  |
| :tabedit file     |     | Edit file in a new tab           |
| :tabfind file     |     | Open file if exists in new tab   |
| :tabclose         |     | Close current tab                |
| :tabs             |     | List all tabs                    |
| :tabfirst         |     | Go to first tab                  |
| :tablast          |     | Go to last tab                   |
| :tabn             |     | Go to next tab                   |
| :tabp             |     | Go to previous tab               |
|                   |     |                                  |

## Editing

| KEYBINDING | ACTION                              |
| ---------- | ----------------------------------- |
| a          | append                              |
| A          | Append from end of line             |
| i          | insert                              |
| o          | Next Line                           |
| O          | Previous Line                       |
| s          | Delete char and insert              |
| S          | Delete Line and insert              |
| C          | Delete until end of line and insert |
| r          | Replace one character               |
| R          | Enter Replace mode                  |
| u          | Undo changes                        |
| `<C-R>`    |    Redo changes                                 |

## Clipboard 

| KEYBINDING      | ACTION                      |
| --------------- | --------------------------- |
| x               | Delete character            |
| dd              | Delete line _(Cut)_         |
| yy              | Yank line _(Copy)_          |
| p               | Paste                       |
| P               | Paste before                |
| `"*p*` / `"+p"` | Paste from system clipboard |
| `"*y` / `"+y`   | Paste to system clipboard                            |

## Search and Replace

| :%s/foo/bar/g | Replace foo with bar in whole document | 
| ------------- | -------------------------------------- |

## Visual Mode

| KEYBINDING         | ACTION                  |
| ------------------ | ----------------------- |
| v                  | Enter visual mode       |
| V                  | Enter visual line mode  |
| `C-v`              | Enter visual block mode |
| ==IN VISUAL MODE== |                         |
| d / x              | Delete selection        |
| s                  | Replace selection       |
| y                  | Yank selection _(Copy)_                        |
For more extensive list of [[Vim]] commands, visit [devhints.io](https://devhints.io/vim).
