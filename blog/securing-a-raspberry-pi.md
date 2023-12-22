# Securing a Raspberry Pi

I use many Raspberry Pi's in production, these are my notes on defaukt security

The command below will run a script that will do the following
- SSH secure config
- Disable Wifi
- Disable Bluetooth
- Install UFW
- Install Fail2Ban

Run this on your Pi
```
curl https://raw.githubusercontent.com/anthonybudd/Secure-Pi/master/secure -sSL | sh
```
