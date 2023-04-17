# ovos-arch-repo
OpenVoice OS Arch Packages Repository

#### How To Use OVOS Arch Repository
**Note**: *WIP* Currently only supports x86_64, more architectures and packages coming soon

**Edit Pacman.conf to add OVOS Repository**
```
sudo nano /etc/pacman.conf
```

**Add OVOS Repository Entry**
**Make sure it matches the following - Copy/Paste As Given**
```
[ovos-arch-repo]
SigLevel = Optional DatabaseOptional
Server = https://github.com/OpenVoiceOS/ovos-arch-repo/raw/main/$arch
```

**Sync and Update**
```
sudo pacman -Sy
```

**Install a package**
```
sudo pacman -S python-ovos-core
```
