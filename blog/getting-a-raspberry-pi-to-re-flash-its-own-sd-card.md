# Getting a Raspberry Pi to re-flash its own SD card

I want to be able to remotely flash a Raspberry Pi's SD card while its running so I wouldn't need to physically remove the SD card each time. Below is a reliable method to re-flash a Raspberry Pi's own SD card. Caution, this will delete all data on the Pi and will restore to a factory version of your chosen OS.

You may need to insall XZ utils `apt-get install xz-utils`

Confirm write location with `lsblk`. It should be `/dev/mmcblk0`

Go to the list of [official Raspberry Pi OS images](https://www.raspberrypi.com/software/operating-systems/) and copy the URL of the .img you would like to flash your SD card with. Currently the URL for the lastest 64-bit full OS is `https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz`. Update the env var `PI_OS_URL` to this value.

⚠️ Use with <b>Extreme</b> caution.
```
export PI_OS_URL=https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz

nice -20 sudo sh -c "echo 1 | sudo tee /proc/sys/kernel/sysrq && curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0 && echo b | sudo tee /proc/sysrq-trigger"
```



```
export PI_OS_URL=https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz

nice -20 sudo sh -c "sudo shutdown -h 10 && curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0"
```