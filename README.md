# Perm
**Contributors:** mayconmesquita  
**License:** GPLv2 or later  
**License URI:** http://www.gnu.org/licenses/gpl-2.0.html  

## Description

A bash tool to abreviate recursive chmod and chown commands.

It can do recursive chmod and chown commands to a valid(s) user and its file(s)/folder(s).

## Install (setup the alias)

```bash
$ sudo chmod +x /path/to/perm
$ sudo ln -s /path/to/perm /usr/local/bin/perm
```

## Usage
```bash
$ sudo perm [permission] [username] [(file) or (--all/-a)]
``` 

## Arguments
`--all/-a` = aplly to all files/folders

`-v` = display version

## Examples

```bash
$ sudo perm 755 root file.txt
```
> >**will do:** chmod -Rf 755 file.txt && chown -Rf 755 root:root file.txt *

```bash
$ sudo perm 755 root --all
```
> >**will do:** chmod -Rf 755 && chown -Rf 755 root:root *

## Contribute

You can contribute to the source code in our [GitHub](https://github.com/mayconmesquita/perm) page.

## Changelog ##

### 1.0.0 ###

* Initial version.

## License

Perm is licensed under [GNU General Public License v2 (or later)](./LICENSE.md).
