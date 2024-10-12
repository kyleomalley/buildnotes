# sudo
```
su -
usermod -aG sudo your_username
```

# nvidia
https://wiki.debian.org/NvidiaGraphicsDrivers#bookworm-535
Note: SecureBoot being enabled will require extra steps to sign the driver. 

```/etc/apt/sources.list
# Debian Bookworm
deb http://deb.debian.org/debian/ bookworm main contrib non-free non-free-firmware
```

# steam

# vscode
``` /etc/apt/sources.d/
deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main
```
