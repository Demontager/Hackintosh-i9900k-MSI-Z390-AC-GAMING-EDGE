# Hackintosh-i9900k-MSI-Z390-AC-GAMING-EDGE

Working Hackintosh configuration running MacOS Monterey 12.6

- Motherboard: MSI-Z390-AC-GAMING-EDGE (MS-7B50) Bios ver. 7B50v1C2
- CPU: Intel i9-9900K Coffee Lake  
- RAM: 64GB 4xKHX3000C15/16GX Kingston DDR4
- Storage: Samsung 970 EVO M.2 512GB  
- iGPU: Intel UHD 630  
- WIFI/BT: Canon Lake PCH CNVi WiFi (Internal)
- SMIBIOS iMac19,1
- OpenCore 0.8.4 RELEASE


![11download](https://user-images.githubusercontent.com/7040503/190868987-2ca863c3-1b9b-4d1f-b69e-75f746fb3b90.png)


## Tested and found working:
- Boot into MacOS 12.6
- Display Port output
- Internal Audio Realtek ALCS1220A
- Sleep Wake up from bluetooth mouse or keyboard
- iGPU hardware acceleration
- WIFI and Bluetooth 
- Internal Network Card

## BIOS SETTINGS
USB Configuration
- USB Controller [Enabled]
- AXHCI Hand-off [Enabled]
- Legacy USB Support [Enabled]

## Integrated Graphics Configuration
- Initiate Graphic Adapter [IGD]
- Integrated Graphics Share memory [64MB]

## PCIe/PCI Sub-system Settings
- Above 4G memory/Crypto Currency mining [Enabled]


Very importan note: Motherboard BIOS has no CFG settings and they are locked by default, this won't allow MacOS to boot at very early stage. To unlock enable these options edit config.plist and set Kernel -> AppleCpuPmCfgLock YES and AppleXcpCfgLock YES 


Note: USBPorts.kext should be configured on target system to fit desired USB ports map. See: Making own USB port map guides below.



## Tools used:
- [Opencore](https://dortania.github.io/OpenCore-Install-Guide/) 
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
- [Hackintool](https://github.com/headkaze/Hackintool)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

## Guides:
- [Custom SSDT's with SSDTTime](https://www.tonymacx86.com/threads/custom-ssdts-using-corpnewts-ssdttime.318976/)
- [Making own USB port map](https://www.tonymacx86.com/threads/the-new-beginners-guide-to-usb-port-configuration.286553/#post-2029768)
- [How to map your USB Ports on macOS](https://elitemacx86.com/threads/how-to-map-your-usb-ports-on-macos.581/)
- [Intel UHD 630 iGPU configuration](https://www.tonymacx86.com/threads/guide-intel-uhd-graphics-630-coffee-lake-headless-mode-main-card.304000/)

## Motherboard backside:
![usb_map_refrence (1)](https://user-images.githubusercontent.com/7040503/190871487-0bde8041-faaf-4d50-8f83-18f75b65ba53.png)


## GeekBench tests:
![geekdownload](https://user-images.githubusercontent.com/7040503/190871525-1cfb46ec-9f95-4dbe-a7da-85da6761637c.png)
![Gpu_geekad](https://user-images.githubusercontent.com/7040503/190871536-7bf29e56-ce41-4f0e-995c-8d80625f74f8.png)


