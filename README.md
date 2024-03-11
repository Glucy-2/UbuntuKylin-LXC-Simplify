# UbuntuKylin-LXC-Simplify
将优麒麟（UbuntuKylin）装到 LXC 容器中可以做的一些精简操作
仅在 22.04 版本上测试
```shell
sudo snap remove --purge firefox
sudo snap remove --purge gnome-42-2204

sudo apt purge --autoremove acpi* network-manager remmina* engrampa* atril* bluez* blueman youker-assistant ubuntu-kylin-software-center kylin-burner cheese* libreoffice* gnome-sudoku gnome-mahjongg gnome-mines thunderbird* onboard* aisleriot pluma usb-creator* gucharmap qtwayland5 fcitx5-module-wayland firefox* ufw ukui-screensaver update-manager*
rm -rf var/log/* root/.bash_history home/*/.bash_hostory var/lib/apt/lists/
```
