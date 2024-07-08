# kad
This is a simple script to run commands and scripts on multiple machines in parallel.

This script assumes you've already set up SSH access on the machines you wish to control.

# General command cheatsheet

``kad execute 'command' group`` - Execute 'command' on machine group 'group'

``kad copy file destination group`` - Copy 'file'(s) to 'destination' on machine group 'group'

``kad help``- Shows this help menu

# Configuring

Machine groups can be defined in ``~/.config/kad/groups`` as an 'array' of IP addresses and usernames following shell syntax.

Example: 
```
servergroup='krum@10.0.0.100 krum@10.0.0.101'
```

# Example commands

``kad execute 'echo hello world' servergroup`` - Executes 'echo hello world' on group 'servergroup'

``kad copy /home/krum/test /home/krum servergroup`` - Copies file 'test' to '/home/krum' on group 'servergroup'

# Todo
```
- A lot.
```
