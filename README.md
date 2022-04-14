# gitswitch

## This repository is no longer maintained.

`gitswitch` now uses a configuration file and has been merged into [phxutils](https://github.com/phx/phxutils).

The new location is [https://github.com/phx/phxutils/tree/master/gitswitch](https://github.com/phx/phxutils/tree/master/gitswitch).

## Old information:

Dependencies:

- `/bin/sh`
- `git`

Easy method for managing multiple `git` identities without changing your normal git paths/commands/configs/etc.

Edit the script as necessary to include your preferred ssh keys, names, and emails.

You can further edit the script to include swapping by profile name, but I will simply switch between 2 identities.

**NOTE:** This script uses `git config --global user.name` and `git config --global user.email`.  If you prefer, feel free to alter the script to not use the `--global` flag.

## Requirements:

Included in `~/.ssh/config`:

```
# BEGIN GIT
Host github.com
  HostName github.com
  User git
  IdentityFile /path/to/rsa_private_key
# END GIT
```

(or whatever git server you are using - just make sure the comments are there.)
