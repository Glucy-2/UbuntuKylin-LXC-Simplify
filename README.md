# UbuntuKylin-LXC-Simplify
将优麒麟（UbuntuKylin）装到 LXC 容器中可以做的一些精简操作
仅在 22.04 版本上测试
```shell
sudo rm -f /etc/update-motd.d/98-fsck-at-reboot
sudo snap remove --purge firefox
# Purge other snap packages
sudo apt purge --autoremove acpi* network-manager remmina* engrampa* atril* bluez* blueman snap* youker-assistant ubuntu-kylin-software-center kylin-burner cheese* libreoffice* gnome-sudoku gnome-mahjongg gnome-mines thunderbird* onboard* aisleriot pluma usb-creator* gucharmap qtwayland5 fcitx5-module-wayland firefox* ufw  update-manager* ukui-power-manager mailcap* xserver-xorg-video* va-driver-all vdpau-driver-all mesa-*-drivers
rm -rf var/log/* snap/ var/snap/ root/snap/ root/.bash_history home/*/.bash_hostory var/lib/apt/lists/ var/cache/*
```
