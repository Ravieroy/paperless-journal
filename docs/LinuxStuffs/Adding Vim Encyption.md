???+ note "Important Info"
	[[Neovim]], which is also known as nvim , does not support encryption.
	Vim v7.4.399 or higher is required 
	*cryptv* feature enabled

## Prerequisites
To see if version of [[Vim]] supports *cryptv*, run the following command within [[Vim]]
```vim
:version
```

If the present version of Vim supports encryption, the following will be displayed in the list of features.
```txt
+cryptv
```

To check what types of encryption are supported by your version of Vim, run:
```vim
:help cryptmethod
```

This will list some or all of the following encryption methods.
- zip
- blowfish
- **blowfish2**
- xchacha20

Vim’s default cryptmethod is blowfish2. To display your Vim’s current cryptmethod, run either of the following equivalent commands.
```vim
:set cryptmethod?
:set cm?
```

Starting with Vim [v8.1.0606](https://github.com/vim/vim/releases/tag/v8.1.0606), the default `cryptmethod` is `blowfish2`. Hence if the Vim version is updated, it should show, 
```vim
cryptmethod=blowfish2
```

If it does not display this, do one of the following.
1. Update Vim version v8.1.0606⁠ or newer.⁠(Recommended)
2. Put the following in `vimrc`.
```bash
set cryptmethod=blowfish2
```

## Using Vim encryption 
**To encrypt a file with Vim:**

1.  Open the file in Vim.
    
2.  In command mode, run `:X` (note that `X` must be upper case).
    
3.  At the `Enter encryption key:` prompt, type a password.
    
4.  At the `Enter same key again:` prompt, retype the password.
    
5.  Save the file.
    
6.  Quit Vim.

**To decrypt, edit, and re-encrypt a file with Vim:**

1.  Attempt to open the file in Vim.
    
2.  At the `Enter encryption key:` prompt, type the file’s password.
    
3.  If you mistyped the file’s password, close the file without saving it and retry. 