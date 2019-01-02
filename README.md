# About
Perm - A bash tool to abreviate recursive chmod and chown commands.

It can do recursive chmod and chown commands to a valid(s) user and its file(s)/folder(s).

# Install (setup the alias)

```bash
$ sudo chmod +x /path/to/perm
$ sudo ln -s /path/to/perm /usr/local/bin/perm
```

# Usage
```bash
$ sudo perm [permission] [username] [(file) or (--all/-a)]
``` 

# Arguments
`--all/-a` = aplly to all files/folders

`-v` = show version

# Examples

```bash
$ sudo perm 755 root file.txt
```
> >**will do:** chmod -Rf 755 file.txt && chown -Rf 755 root:root file.txt *

```bash
$ sudo perm 755 root --all
```
> >**will do:** chmod -Rf 755 && chown -Rf 755 root:root *

# Changelog

v0.1.0 - Initial release
