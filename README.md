# dystopia

This is my arch package repo

## Enable

- To enable it, put the following in your `/etc/pacman.conf`
  
```conf
[dystopia]
SigLevel = Required DatabaseOptional
Server = https://github.com/DemonKingSwarn/$repo/raw/refs/heads/master/$arch
```
 
 - do `pacman -Sy` to update and sync the repositories

`NOTE:` Pacman will complain about importing a PGP key that is either invalid or corrupted. The problem can be fixed locally signing the imported key:

```sh
sudo pacman-key --lsign-key 6F189D2A8EAFB02D692C7919A3BEF7FBBF49B562
```
