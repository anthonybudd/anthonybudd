# Getting a Raspberry Pi to re-flash its own SD card

I wanted to be able to remotely flash a Raspberry Pi's SD card so I would not need to physically remove the SD card each time.

You may need to insall XZ utils
`apt-get install xz-utils`

Confirm write location with 
`lsblk`
It should be `/dev/mmcblk0`

Go to the list of [offical Raspberry Pi operating system images](https://www.raspberrypi.com/software/operating-systems/) and copy the URL of the .img you would like to flash your SD card with. For me the lastest 64-bit Full os is `https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz`

⚠️ Use with caution.
```
echo 1 | sudo tee /proc/sys/kernel/sysrq

export PI_OS_URL=https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz && \ 

nice -20 sudo sh -c "curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0 && echo b | sudo tee /proc/sysrq-trigger"
```