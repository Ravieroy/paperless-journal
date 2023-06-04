**dmesg** command also called as “driver message” or “display message” is used to examine the kernel ring buffer and print the message buffer of kernel. The output of this command contains the messages produced by the device drivers.

```bash
Show kernel messages:

      dmesg

  Show kernel error messages:

      dmesg --level err

  Show kernel messages and keep reading new ones, similar to `tail -f` (available in kernels 3.5.0 and newer):

      dmesg -w

  Show how much physical memory is available on this system:

      dmesg | grep -i memory

  Show kernel messages 1 page at a time:

      dmesg | less

  Show kernel messages with a timestamp (available in kernels 3.5.0 and newer):

      dmesg -T

  Show kernel messages in human-readable form (available in kernels 3.5.0 and newer):

      dmesg -H

  Colorize output (available in kernels 3.5.0 and newer):

      dmesg -L
```

