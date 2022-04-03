# Opencore-HP-Elitebook-840-G3
A repository of Opencore configuration made for the HP Elitebook 840 G3

## DISCLAIMER 
I will not be held responsible for any damage, permanent loss of data or any sorts of consequences that may arise by using my configuration files on your devices. Please use at your own risk.

## Current Release
- Opencore 0.7.9
- Monterey 12.3
- All latest kexts as of March 31, 2022

## Notebook Specifications

| Specification  | Model |  Remark  |
| ------------- | ------------- | ------------- |
| Chipset  | Intel | N75 v01.52 (4/20/2021) |
| CPU  | Intel i5-6300U  |
| iGPU  | Intel HD Graphics 520 | 
| Storage  | Samsung Evo 870 SATA 2.5 256GB  |
| RAM  | 16GB (2x8GB)2133 MHz DDR4 |
| Ethernet  | Intel I219-LM  |
| Wi-Fi  | Fenvi (BCM94360NG)  |
| Bluetooth  | Fenvi (BCM94360NG)   |
| Audio  | Conexant HD (layout 13)   |
| Trackpad | Synaptics SMBus Touchpad   |
| Inputs | HP PS2 Kbd/Mouse   |


## What's working
- Mostly everything
- AppleID and iServices
- Wi-Fi & Bluetooth, Ethernet
- Display outputs DP
- Speaker, Headphone jack, microphone
- USB ports mapping
- Sleep/wake/shutdown
- Keyboard backlighting
- All Continuity & Handoff features (need to have Apple native WLAN card.

## What's not working
- SD Card reader
- Fingerprint Reader

## Not tested
- VGA output
- SIM card slot
- Smart card
- Docking station

## Quirks/issues
- Possible issue with RTC especially if dual booting with other OS.
- Enabling Quirk "DisableRTCChecksum" does not fix the issue
- I have included the RTCMemoryFixup.kext but it is disabled in config.plist as I'm still working on it.
- I will update the repo once i find a more permanent fix for this

## Bios Settings
- Security > Disable Intel Software Guard Extensions (SGX)
- Advanced >
  - Boot Options > Disable Fast Boot
  - Secure Boot Configurations > Legacy Support Disable and Secure Boot Disable
  - System Options > Enable: Hyperthreading, Virtualization Technology (VTx)
  - System Options > Disable: Virtualization Technology for Directed I/O (VTd)

## Credits
- All credits & rights goes to the maintainers, contributors and developers of the Opencore project and respective kernel extensions.
- Apple Inc.
