# RPI-headless-install
tuto pour installer rpi os sans ecran

  - Install raspberry pi OS 
  - Write an empty text file named "ssh" (no file extension) to the root of the directory of the card. When it sees the "ssh" on its first boot-up, Raspberry Pi OS will automatically enable SSH (Secure Socket Shell), which will allow you to remotely access the Pi command line from your PC.
  - Create a text file called wpa_supplicant.conf, and place it in the root directory of the microSD card. You will need the following text in the file.
```
country=FR
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
scan_ssid=1
ssid="your_wifi_ssid"
psk="your_wifi_password"
}
```
