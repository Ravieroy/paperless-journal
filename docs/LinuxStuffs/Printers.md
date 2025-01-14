Before Configuring the Default Printer in Linux check with lpstat command
```bash
lpstat -t
```

Set Default Printer Linux [[Terminal]]
```bash
lpoptions -d <Printer Name>
```

We can also setup an default printer using simple environment variable adding into user profile file called `~/.bashrc`
```bash
export PRINTER=printer-name
```


## Displaying printer settings

```bash
lpoptions | tr " " '\n'
```

With the **-v** option, the **lpinfo** command will list drivers and related information.

```bash
lpinfo -v
```

The `lpoptions` command will show the settings of the default printer. Use the `-p` option to specify one of a number of available printers.

```bash
lpoptions -p <Printer Name>
```

## Useful commands

1. To print a document on the default printer, just use the `lp` command followed by the name of the file you want to print.
```bash
lp fileName.pdf
```

2. The `lpq` command displays the print queue.
3. With the **-n** option, the `lp` command allows to specify the number of copies of a printout we  want. `lp -n 11 fileName` 
4. To cancel a print job, we can use the `cancel` or `lprm` command.
5. To print in two-sided mode,  use
```bash
lp -o sides=two-sided-long-edge fileName.pdf
```
6. If we want all of our documents to print in two-side mode, we can change our `lp` settings by using the `lpoptions` command to change the setting for `sides`.
```bash
lpoptions -o sides=two-sided-short-edge
```
