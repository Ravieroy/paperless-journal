Terminal is one of the most powerful programs on Linux. The terminal emulator allows an end-user to access the console as well as its applications such as text user interface and command-line interface. Some of the most used terminal emulators are mentioned below. 

### 1. Terminator 
Inorder to install Terminator, we can use default [[Package manager]], 
*For Debian/Ubuntu based distros*
```bash
sudo apt install terminator
```

For Fedora
```bash
sudo dnf install terminator
```

### 2.  Kitty 

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
|                |        |                                   |            |