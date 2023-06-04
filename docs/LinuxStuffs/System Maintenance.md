- ## shutdown
Shutdown and reboot the system.

```bash
Power off (halt) immediately:

      shutdown -h now

  Reboot immediately:

      shutdown -r now

  Reboot in 5 minutes:

      shutdown -r +5 &

  Shutdown at 1:00 pm (Uses 24h clock):

      shutdown -h 13:00

  Cancel a pending shutdown/reboot operation:

      shutdown -c
```

- ## reboot
Reboot the system.

```bash
Reboot the system:

      reboot

  Power off the system (same as `poweroff`):

      reboot --poweroff

  Halt the system (same as `halt`):

      reboot --halt

  Reboot immediately without contacting the system manager:

      reboot --force

  Write the wtmp shutdown entry without rebooting the system:

      reboot --wtmp-only
```

- ## halt
```bash
Halt the system:

      halt

  Power off the system (same as `poweroff`):

      halt --poweroff

  Reboot the system (same as `reboot`):

      halt --reboot

  Halt immediately without contacting the system manager:

      halt --force --force

  Write the wtmp shutdown entry without halting the system:

      halt --wtmp-only
```

