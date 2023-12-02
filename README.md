# Thinkpad L15 G1 Hackintosh Intel I5 10210U
Hackintosh for L15 G1 Thinkpad Comet Lake

![image](https://github.com/kefrulz/Thinkpad-L15-Hackintosh/blob/03a9c5608330700fa99e760cb3617074f0b84706/Screenshot%202023-12-02%20at%2014.49.38.png)


### An OpenCore config for Lenovo Thinkpad L15 G1 Thinkpad ###
This is work in progress, i will post updates as soon as i figure things out

I am also open to suggestions from all of you to improve MacOS on this laptop.

For any troubleshooting please follow the great Dortania guide
* https://dortania.github.io/OpenCore-Install-Guide/

## OpenCore version: 0.9.6 ##

## macOS: 13.6.1 ##

## SPECS: ##
* LAPTOP: Thinkpad L15 G1
* CPU: Intel I5 10210U
* Display: Intel UHD Graphics 620
* Network: BCM94360CS2 (From broken Macbook air 2015 with NGFF adapter // Can also work with stock card. Just install Intel KEXT from here https://github.com/OpenIntelWireless/itlwm )
* Hard-disk: Toshiba 256 NVME
* RAM: 16GB
* Please change MLB/ROM/Serial Number/UUID.

## WORKING: ##
Everything works great

## Installation instructions: ##
* Download EFI from this repo
* Download OCAT https://github.com/ic005k/OCAuxiliaryTools
* Open Config in OCAT and go to PI(Platform Info) and generate a new System Product Name (This will generate all Paltform Info details for your new Hackintosh) and then Save (Don't worry about any errors in Validation, they show up since when you download OCAT it does not have latest OpenCore version attached. OPTIONAL: To solve this go to OCAT>Upgrade OpenCore and Kexts and press on Get latest version of Opencore) Then Save.
* Download Open Core Legacy Patcher on another working MAC
* Download Monterey/Ventura
* Create the USB installer (skip installing of OCLP EFI)
* Download https://github.com/benbaker76/EFI-Agent to mount the EFI
* Paste the EFI from this repo
* Boot from USB
* Select Monterey installer (DMG)
* Follow Setup
* Format Disk as APFS - GUID (if you have issues, just format first to ExFAT - MBR and then to APFS - GUID)
* Install MACOS
* Boot again from USB - Select MACOS installer
* Do this as many times needed until the Disk name you selected earlier when formatting appeares
* Enjoy your Hackintosh :)

## Post Install: ##
* Download EFI Agent to mount the Internal Drive EFI
* Copy the EFI folder from the USB drive / Download again from here to the Internal Disk EFI


## Bios settings: ##
* Enable Secure boot


## Not working yet: ##
* you tell me :)

Happy Hackintoshing :)
