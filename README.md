# UbuntuKylin-LXC-Simplify

将优麒麟（UbuntuKylin）装到 LXC 容器中可以做的一些精简操作

仅在 22.04 版本上测试

```shell
cd /
sudo rm -f /etc/update-motd.d/98-fsck-at-reboot
echo | sudo tee etc/fstab
sudo snap remove --purge firefox
# Purge other snap packages
sudo apt install ssl-cert zstd p7zip
sudo apt purge --autoremove acpi* apparmor network-manager ppp* modemmanager iptables nftables wpasupplicant remmina* engrampa* atril* bluez* blueman snap* youker-assistant ubuntu-kylin-software-center kylin-burner cheese* libreoffice* samba samba-common python3-samba speech-dispatcher* guile* gnome-sudoku gnome-mahjongg gnome-mines thunderbird* onboard* aisleriot pluma usb-creator* gucharmap qtwayland5 fcitx5-module-wayland firefox* ufw rtkit update-manager* ukui-power-manager mailcap* xserver-xorg-video* va-driver-all vdpau-driver-all mesa-*-drivers ukui-screensaver cups* openprinting-ppds printer-driver* python3-cups* system-config-printer*
sudo dpkg -r --force-all i965-va-driver intel-media-va-driver
sudo rm -rf var/cache/* var/backups/* var/crash/* var/log/* snap/ var/snap/ root/snap/ root/.bash_history home/*/.bash_hostory root/.cache/* home/*/.cache/* root/.log/* home/*/.log/* root/.config/* home/*/.config/* root/.dubs/* home/*/.dubs/* root/.vnc/*.log home/*/.vnc/*.log root/.vnc/*.pid home/*/.vnc/*.pid var/lib/apt/lists/ usr/lib/libreoffice/ etc/libreoffice/ usr/share/fonts/truetype/libreoffice/ usr/share/bash-completion/completions/ var/lib/samba/ usr/share/grub/
```
