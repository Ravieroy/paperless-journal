## Fonts Installation
This explains the installation of `powerline fonts` which will fix the weird glyphs in [[Oh-My-Zsh Installation]] ( [Source](https://powerline.readthedocs.io/en/1.0/installation/linux.html)).

**Step 1: Download the latest version of the symbol font and fontconfig file:**
```bash
wget https://github.com/Lokaltog/powerline/raw/develop/font/PowerlineSymbols.otf
wget https://github.com/Lokaltog/powerline/raw/develop/font/10-powerline-symbols.conf
```

!!! tip
***Make sure following folders exists. If not, make it manually.*** 
- ~/.fonts/ 
- ~/.config/fontconfig/conf.d/

**Step 2: Move the symbol font to a valid X font path**

```bash
mv PowerlineSymbols.otf ~/.fonts/
mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
```

**Step 3: Update font cache**

```bash
fc-cache -vf ~/.fonts/
```

 Finally, close all instances of the terminal emulator and reopen it.

!!! tip
 ***For any kind of fonts like [Nerd Font,](https://www.nerdfonts.com/) simply get the font file which will be in compressed format. Just extract the folder and move it to the `.fonts` directory.***

---
