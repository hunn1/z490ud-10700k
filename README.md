# OpenCore on Gigabyte Z490 UD + i7 10700K + iGPU


## OpenCore version

0.7.1

# Comet Lake（桌面端，第十代酷睿）

Comet Lake 平台建议安装 macOS 10.15.5 及以上
BIOS 设置


## 关闭

Fast Boot
Secure Boot
VT-d（可以开启，前提是 DisableIoMapper 设置为 Yes）
CSM
Thunderbolt（全新安装时不当配置雷电接口可能造成问题，建议安装完成后再开启调试）
Intel SGX Intel Platform Trust
Intel Platform Trust
CFG Lock（MSR 0xE2 写保护）此项必须关闭，如果你的 BIOS 里没有此项，注意设置 AppleCpuPmCfgLock 和 Apple XcpmCfgLock 为 Yes。


## 开启


VT-x
Above 4G decoding
Hyper-Threading
Execute Disable Bit
EHCI/XHCI Hand-off
OS type：Other（如果你选择 Other 会导致 CSM 联动开启，选择 Windows 8.1/10 UEFI Mode）
DVMT Pre-Allocated：64MB 及以上


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


