# OpenCore-CUBE-Thinker-i35
OpenCore for CUBE Thinker/i35

## OC information
* OC Version: 0.5.9
* Tested OS Version: 10.15.5

## Working
* WIFI (*Modify `EFI/OC/Kexts/itlwm.kext/Contents/Info.plist` to set your WiFi SSID and password.*)
* Bluetooth
* Sidecar
* Touch Screen
* Trim

## Not working
* Trackpad
* Sleep

## Before installation
### Edit config.plist
Using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate SMBIOS information and write config.plist

### BIOS Settings
#### Disable

* Fast Boot
* Secure Boot
* Compatibility Support Module (CSM)
* Intel Platform Trust

#### Enable
* Above 4G decoding

#### Set
##### Chipset -> Graphics Configuration
* Aperture Size 512M
* DVMT Pre-Allocated 64M
* DVMT Total Gfx Mem MAX

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html)

## Credits
[zxystd/itlwm](https://github.com/zxystd/itlwm)

[zxystd/IntelBluetoothFirmware](https://github.com/zxystd/IntelBluetoothFirmware)