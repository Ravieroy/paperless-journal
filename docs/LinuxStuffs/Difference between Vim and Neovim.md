# Difference between Vim and Neovim
[Video Link](https://www.youtube.com/watch?v=K-hP727tv6E) for More

[[Vim]] and [[Neovim]] are two screen-based text editors. To overcome the issues with Vim, Neovim was developed to expand on the core functionalities of Vim and for users who want to make the best out of vim.

## Installation Directory 
Both follow different conventions on where to store their configuration files. Vim likes to store current user files in the `~/.vim/` directory and the user-specific configuration files in the `~/.vimrc` home directory. Your home directory is specified with `$HOME`. Neovim, on the other hand, adheres to the XDG base directory specification and stores all its configuration files in the `~/.config` directory. The Neovim configuration is stored inside the `~/.config/nvim` directory.

## Plug-In System
Vim’s plug-in API is restrictive and cumbersome. Neovim is a complete rework of the Vim text editor with a fully redesigned yet sophisticated plug-in architecture that has more powerful plugins than before. Most plugins written for Vim also work just fine in Neovim. Read [[Install Vim plugins]]

## Project Management 
Bram Moolenaar, the developer for [[vim]] takes up a benevolent dictator for life situation, which means he has absolute control over every single feature that goes into the code of `vim`. While there are a  huge number of developers who help with the vim code, but eventually Bram is the one who is responsible for making sure the features are added and delivered to the users. Vim's development is discussed via a mailing list. 

[[Neovim]] on the other hand has an extensive database on GitHub outlining the process of contributing to Neovim. It does make the use of benevolent dictator for life situation

## Lua Support 
Both Vim and Neovim supports plugins in Lua, however on Vim, Lua is just another programming language. In Neovim , Lua is a first class citizen, i.e everything can be done in Lua instead of writing vim scripts in vimrc. 


 

