# apt install
apt install yq -y

# /etc/apt/sources.list
```
deb http://deb.debian.org/debian bookworm contrib main non-free-firmware
deb http://deb.debian.org/debian bookworm-updates contrib main non-free-firmware
deb http://deb.debian.org/debian bookworm-backports contrib main non-free-firmware
deb http://deb.debian.org/debian-security bookworm-security contrib main non-free-firmware

deb http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware

```

# sudo
```
su -
usermod -aG sudo your_username
```

# nvidia
https://wiki.debian.org/NvidiaGraphicsDrivers#bookworm-535
Note: SecureBoot being enabled will require extra steps to sign the driver (via dkms).

# steam

https://wiki.debian.org/Steam

# vscode
``` /etc/apt/sources.d/
deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main
```

# Github Desktop (shiftkey)
```
wget -qO - https://apt.packages.shiftkey.dev/gpg.key | gpg --dearmor | sudo tee /usr/share/keyrings/shiftkey-packages.gpg > /dev/null
sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/shiftkey-packages.gpg] https://apt.packages.shiftkey.dev/ubuntu/ any main" > /etc/apt/sources.list.d/shiftkey-packages.list'

sudo apt update && sudo apt install github-desktop
```

## vscode extensions
    Code Runner: For running code snippets easily.
    GitLens: Enhances Git capabilities in VSCode.

# Keyboard Settings
