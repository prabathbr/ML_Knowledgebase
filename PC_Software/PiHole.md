Debain 11 32bit i386 : https://cdimage.debian.org/debian-cd/current/i386/iso-dvd/  

Debain Guide : https://www.debian.org/releases/stretch/i386/ch06s03.html.en#pkgsel  

comment CDROM in /etc/apt/sources.list, apt update  

remore libreoffice : apt purge libreoffice-common  

https://github.com/brektrou/rtl8821CU  
https://github.com/kelebek333/rtl8821CU/tree/buildfix-518  

https://github.com/tomaspinho/rtl8821ce#ubuntu--debian   
sudo ./dkms-install.sh  

don't do dkms, just use manual installation steps  

sudo usb_modeswitch -KW -v 0bda -p c811  

sudo nano /lib/udev/rules.d/40-usb_modeswitch.rules 

```
# Realtek 8811CU Wifi AC USB
ATTR{idVendor}=="0bda", ATTR{idProduct}=="1a2b", RUN+="usb_modeswitch -K -v 0bda -p 1a2b"  
```

Bus 001 Device 009: ID 0bda:1a2b Realtek Semiconductor Corp. RTL8188GU 802.11n WLAN Adapter (Driver CDROM Mode)  
Bus 001 Device 011: ID 0bda:c811 Realtek Semiconductor Corp. 802.11ac NIC

apt install neofetch  

```
 neofetch
       _,met$$$$$gg.          wyseuser@wyse
    ,g$$$$$$$$$$$$$$$P.       -------------
  ,g$$P"     """Y$$.".        OS: Debian GNU/Linux 11 (bullseye) i686
 ,$$P'              `$$$.     Host: C CLASS Rev1
',$$P       ,ggs.     `$$b:   Kernel: 5.10.0-18-686-pae
`d$$'     ,$P"'   .    $$$    Uptime: 40 mins
 $$P      d$'     ,    $$P    Packages: 1335 (dpkg)
 $$:      $$.   -    ,d$$'    Shell: bash 5.1.4
 $$;      Y$b._   _,d$P'      Terminal: /dev/pts/1
 Y$$.    `.`"Y$$$$P"'         CPU: VIA Eden 1000MHz (1) @ 1.000GHz
 `$$b      "-.__              GPU: 00:01.0 VIA Technologies, Inc. VX855/VX875 Chrome 9 HCM Integrated Graphics
  `Y$$                        Memory: 154MiB / 1759MiB
   `Y$$.
     `$$b.
       `Y$$b.
          `"Y$b._
              `"""

```

curl -sSL https://install.pi-hole.net | bash  

https://docs.pi-hole.net/main/basic-install/  

