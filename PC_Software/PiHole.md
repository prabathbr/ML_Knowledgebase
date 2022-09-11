Debain 11 32bit i386 : https://cdimage.debian.org/debian-cd/current/i386/iso-dvd/  

Debain Guide : https://www.debian.org/releases/stretch/i386/ch06s03.html.en#pkgsel  

comment CDROM in /etc/apt/sources.list, apt update  

remore libreoffice : apt purge libreoffice-common  

https://github.com/brektrou/rtl8821CU  
sudo make dkms_install  

sudo usb_modeswitch -KW -v 0bda -p c811  

sudo nano /lib/udev/rules.d/40-usb_modeswitch.rules 

`# Realtek 8811CU Wifi AC USB`
ATTR{idVendor}=="0bda", ATTR{idProduct}=="1a2b", RUN+="usb_modeswitch -K -v 0bda -p 1a2b"  

Bus 001 Device 009: ID 0bda:1a2b Realtek Semiconductor Corp. RTL8188GU 802.11n WLAN Adapter (Driver CDROM Mode)
Bus 001 Device 011: ID 0bda:c811 Realtek Semiconductor Corp. 802.11ac NIC

