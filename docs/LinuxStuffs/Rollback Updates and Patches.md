## Fedora/RHEL based distros 

### Rollback single package/update

1. Check history:
```bash
dnf history
```

2. Rollback
```bash
dnf history undo <ID>
```

Where, `<id>` is the ID provided by the history. 
