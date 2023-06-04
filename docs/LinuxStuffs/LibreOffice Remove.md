# Remove bundled LibreOffice
LibreOffice 7.x can be installed alongside older LibreOffice versions, but conflicts may occur.

To remove prior installations of LibreOffice:
`sudo apt remove libreoffice-common`

If you also want to remove LibreOffice configuration files, use the purge switch:
`sudo apt purge libreoffice-common`

Note that you could also use `remove --purge`, which is is equivalent to the purge command.

Remove unused dependencies:

`sudo apt autoremove`
