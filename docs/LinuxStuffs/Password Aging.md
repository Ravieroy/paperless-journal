- Command : `chage`
- Syntax
```bash
chage [-m mindays] [-M maxdays] [-d lastday] [-I inactive] [-E expiredate] [-W warndays] user
```

`-d` : Days since Jan 1, 1970 that password was last changed. 
`-m` : The minimum number of days required before the password can be changed by user.(0 means no limit and password can be changed anytime)
`-M` : The maximum number of days for which the password is valid. (for e.g., 90 would mean password has to be changed after 3 months)
`-W` : The number of days before the password expiry date, that the user is warned of the password change.
`-I` : The number of days after the password expires that the account is disabled.
`-E `: Days since Jan 1, 1970 that account is disabled.

- File = /etc/login.defs

-  `PASS_MAX_DAYS    99999`

- `PASS_MIN_DAYS    0`

- `PASS_MIN_LEN    5`

- `PASS_WARN_AGE    7`

- Examples 

  - List password information for the user:
    `chage --list username`

  - Enable password expiration in 10 days:
    `sudo chage --maxdays 10 username`

  - Disable password expiration:
    `sudo chage --maxdays -1 username`

  - Set account expiration date:
    `sudo chage --expiredate YYYY-MM-DD username`

  - Force user to change password on next log in:
    `sudo chage --lastday 0 username`

