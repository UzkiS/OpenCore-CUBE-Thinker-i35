# OpenCore-CUBE-Thinker-i35
OpenCore for CUBE Thinker/i35

## OC information
* OC Version: 0.6.7
* Tested OS Version: 10.15.6

## Working
* WIFI
* Bluetooth
* Sidecar
* Touch Screen
* Trim

## Not working
* Trackpad
* Sleep

## Before installation
### Edit config.plist
Using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate SMBIOS information(chose the MacBookPro14,1 SMBIOS) and write config.plist

* The Type part gets copied to Generic -> SystemProductName.

* The Serial part gets copied to Generic -> SystemSerialNumber.

* The Board Serial part gets copied to Generic -> MLB.

* The SmUUID part gets copied to Generic -> SystemUUID.

### BIOS Settings
#### Disable

* Boot -> Fast Boot
* Security -> Secure Boot -> Attempt Secure Boot
* Advanced -> CSM Configuration -> CSM Support
* Intel Platform Trust

#### Enable
* Advanced ->  PCI Subsystem Settings -> Above 4G decoding

#### Set
##### Chipset -> System Agent (SA) Configuration -> Graphics Configuration
* Aperture Size 512M
* DVMT Pre-Allocated 64M
* DVMT Total Gfx Mem MAX

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

## Kext information
| Name                             | Version |
| -------------------------------- | ------- |
| Lilu                             | 1.5.1   |
| VirtualSMC                       | 1.2.1   |
| WhateverGreen                    | 1.4.8   |
| AppleALC                         | 1.5.8   |
| AirportItlwm                     | 1.3.0   |
