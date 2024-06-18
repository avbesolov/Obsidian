#### snap
Snap – это название системы упаковки и развертывания ПО. Snaps – это название пакетов, а snapd – это название инструмента для работы с этими пакетами.

**install snap subsystem**
```
dnf install snapd
```

**install a snap**
```
snap install <snap>
```

**find snap**
```
snap find <search>
```

**list installed snaps**
```
snap list
```

**upgrade and downgrade Snap packages**
```
sudo snap refresh <package>
sudo snap refresh --list # show snaps that have updates available
sudo snap revert <package> # revert to previous version
```

**remove snap**
```
sudo snap remove <package>
sudo snap remove --purge <package> # remove snap related files/configs
```

**change snap channel**
```
sudo snap refresh <package> --channel=<stable,candidate,beta,edge,etc> 
```

**install offline**
```
snap download <package_name> # may need to download and install snap subsystem ie gnome-3-26-1604
snap ack <package_name.assert>
snap install <package_name.snap>
```
