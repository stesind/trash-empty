# gnome-trash-empty
Gnome does not empty trash files on ZFS file systems. This service and timer do daily.

# Install
 
```shell
# Ubuntu/Debian
sudo apt install trash-cli
# Arch Linux
sudo pacman -S trash-cli

git clone https://github.com/stesind/gnome-trash-empty.git
cd gnome-trash-empty

install -m 644 -o root -g root trash-empty.service /etc/systemd/system
install -m 644 -o root -g root trash-empty.timer /etc/systemd/system

```
Change the default daily frequency according your needs.
