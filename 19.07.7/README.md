# OpenWrt 19.07.7 (Terbaru) untuk GL-iNet GL-MT300N-V2

## Luci / Putty / WinSCP / MobaXterm
- IP Address : <a href="http://192.168.1.1">192.168.1.1</a>
- Username : root
- Password : goodlife
- Password Wifi Openwrt : goodlife

## Aplikasi :
- Suport Modem Hilink ( eth1 ) :
  - Tested Huawei E3372
- Suport Modem 3G ( 3g-3g )
- Suport Modem 4G ( wwan0 )
- Suport Tethering HP ( usb0 )
- htop ( Buat liat running program d CPU ataupun RAM )
- https-dns-proxy ( Membuka situs yang di blokir, buka https://dnsleaktest.com/ DNS akan berubah ke Cisco OpenDNS)
- Adblock ( Memblockir Iklan-iklan Web )
- OpenVPN-OpenSSL GUI
- WireGuard VPN 
- L2TP

## Cara Install :
- Upload Backup openwrt-19.07.7-ramips-mt76x8-gl-mt300n-v2-squashfs-sysupgrade.bin via WinSCP / MobaXterm di /tmp
- Rename Backup openwrt-19.07.7-ramips-mt76x8-gl-mt300n-v2-squashfs-sysupgrade.bin ke factory.bin
- Via Putty / MobaXterm :
```sh
cd /tmp && mtd -e firmware -r write factory.bin firmware
```
- WiFi langsung on setelah di Flash, kalo belum hidup tunggu +- 3 menitan
- Free Space :
  - Luci - System - Software = 48% ( 6.0 MB )
