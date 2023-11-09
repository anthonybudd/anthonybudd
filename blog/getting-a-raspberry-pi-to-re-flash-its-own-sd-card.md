# Getting a Raspberry Pi to re-flash its own SD card

<p align="center">
  <img width="auto" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/main/img/sd-cards.png" alt="SD Cards">
</p>

I want to be able to remotely flash a Raspberry Pi's SD card while its running so I wouldn't need to physically remove the SD card each time. Below is a reliable method to re-flash a Raspberry Pi's own SD card. Caution, this will delete all data on the Pi and will restore to a factory version of your chosen OS.

You may need to insall XZ utils with the command `apt-get install xz-utils` but this comes pre-installed with the latest version of Raspberry Pi OS.

Confirm write location with `lsblk`. It should be `/dev/mmcblk0`

Go to the list of [official Raspberry Pi OS images](https://www.raspberrypi.com/software/operating-systems/) and copy the URL of the .img you would like to flash your SD card with. Currently the URL for the lastest 64-bit full OS is `https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz`. Update the env var `PI_OS_URL` to this value.

⚠️ Use with <b>Extreme</b> caution.
```
export PI_OS_URL=https://downloads.raspberrypi.com/raspios_arm64/images/raspios_arm64-2023-10-10/2023-10-10-raspios-bookworm-arm64.img.xz

nice -20 sudo sh -c "sudo shutdown -h 15 && curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0"
```

### Why I used `sudo shutdown -h 15`
While working on this I discovered that you cannot reboot the Pi after you've re-flashed the SD card. I tried `reboot`, `shutdown` and  `echo b > /proc/sysrq-trigger` but none of these work because there are no users in the linux user database anymore. To get arround this you need to schedule a reboot before you `dd`. The obvious downside to this solution is that you need to guess the right delay ahead of time, too short and the flash will fail, bricking the SD card. You could mitigate this risk by pre-downloading your image, this would also have security benifits. The solution I have implimented is not perfect but it works.

Note: The code below does not work.
```
nice -20 sudo sh -c "curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0 && echo b | sudo reboot -f"

# OR 

nice -20 sudo sh -c "echo 1 | sudo tee /proc/sys/kernel/sysrq && curl -L $PI_OS_URL | xz -d | sudo dd bs=4M of=/dev/mmcblk0 && echo b | sudo tee /proc/sysrq-trigger"
```