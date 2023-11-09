# Getting a Raspberry Pi to re-flash its own SD card





```
export PI_OS_URL=https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz && \ 
curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0 && \
sudo reboot -f
```