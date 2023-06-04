Terminal is one of the most powerful programs on Linux. The terminal emulator allows an end-user to access the console as well as its applications such as text user interface and command-line interface. Some of the most used terminal emulators are mentioned below. 

### 1. Terminal Commands

- `clear` : Clears your screen
- `exit` : Exit out of the shell or a user session
- `script` : This command stores terminal activities in a log file that can be named by a user. When a name is not provided by the user, the default filename *typescript* is used.

```bash
Record a new session to a file named `typescript` in the current directory:

      script

  Record a new session to a custom filepath:

      script path/to/session.out

  Record a new session, appending to an existing file:

      script -a path/to/session.out

  Record timing information (data is outputted to the standard error):

      script -t 2> path/to/timingfile
```

### 2. Terminator

Inorder to install Terminator, we can use default [[Package Manager]], 
*For Debian/Ubuntu based distros*
```bash
sudo apt install terminator
```

For Fedora
```bash
sudo dnf install terminator
```

### 3.  Kitty 

*For Debian/Ubuntu based distros*
```bash
sudo apt install kitty
```

For Fedora
```bash
sudo dnf install kitty
```

There are preinstalled terminal emulator in every [[Linux distros]] which can be used similar to any other terminal emulators of choice. Some of the common terminal shortcuts are mentioned below.

| SCREEN OUTPUT |        | CURSOR MOVEMENT         |         |
| ------------- | ------ | ----------------------- | ------- |
| Clear Screen  | ctrl+L | Go to start Of The Line | ctrl+a  |
| Pause Output  | ctrl+s | Go to end Of The Line   | ctrl+e  |
| Resume Output | ctrl+q | Go one word back        | ctrl+Left Arrow |
| Exit terminal | ctrl+d | Go one word forward     | ctrl+Right Arrow |
|               |        |                         |         |

| DELETE                        |        | EDITING                         |        |
| ----------------------------- | ------ | ------------------------------- | ------ |
| Delete character under cursor | ctrl+d | Transpose adjacent characters   | ctrl+t |
| Delete from end to cursor     | ctrl+k | Change to U-case(cursor to end) | Esc+u  |
| Delete everything             | ctrl+u |                                 |        |

| SEARCH         |        | BASH BANG                         |            |
| -------------- | ------ | --------------------------------- | ---------- |
| Reverse Search | ctrl+r | Execute last Command              | !!         |
| Forward Search | ctrl+s | Execute most Recent "command"     | !`<com>`   |
| Quit Search    | ctrl+g | Displays "command" to be Executed | !`<com>`:p |
|                |        |                                   |            |

| KEY |     | ACTION               |
| ---------- | --- | -------------------- |
| CTRL-u         |     | Erase everything to start of the line          |
| CTRL-c        |     | Stop or kill a command      |
| CTRL-z         |     |  Suspend or put in background                |
| CTRL-d   |     | Exit out of interactive program |
| CTRL-k     |     | Erase everything to the end of the line        |
|            |     |                      |


