# OpenCore on Gigabyte Z490 UD + i7 10700K + iGPU


## OpenCore version

0.7.1


# BIOS Features
## Disabled

Fast Boot
Secure Boot
VT-d
SuperIO
Serial Port [ fixes stuttering ]
Legacy USB Support

## Enabled

4G Decoding
Re-size BAR support: Auto
Hyper-threading
CSM Support [my system won't properly boot without this on due to the GPU]
Windows 10 Features: Other
Storage Boot Option Control - UEFI

## OS

macOS Big Sur 11.5.1
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/001.png>


## network setting
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/002.png>

## tests

### CPU turbo 

<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/CPUS.jpg>

### intel power

<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/intel_power.jpg>


### istat menu

<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/CPU.png>
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/RAM.png>
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/SENSORS.png>


### cinebench
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/cinebench.jpg>

### htop
<img src=https://github.com/hunn1/z490ud-10700k/blob/main/images/htop.png>


## What Works

- Sleep
- USB
- Audio
- Ethernet （RTL8111 100M）
- USB Bluetoth (免驱的)
- AirDrop （能用是正常的）
- iMessages {记得换三码，不换原地爆炸}
- HDMI Audio
- HIDPI 



## Credits

<a href=https://github.com/tiny0little/Gigabyte-Z490-UD-OC>tiny0little/Gigabyte-Z490-UD-OC</a><br>


