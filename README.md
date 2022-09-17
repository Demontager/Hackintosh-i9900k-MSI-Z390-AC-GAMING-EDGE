# Hackintosh-i9900k-MSI-Z390-AC-GAMING-EDGE

Working Hackintosh configuration running MacOS Monterey 12.6

- Motherboard: MSI-Z390-AC-GAMING-EDGE (MS-7B50) Bios ver. 7B50v1C2
- CPU: i9-9900K  
- RAM: 64GB 4xKHX3000C15/16GX Kingston DDR4
- Storage: Samsung 970 EVO M.2 512MB  
- iGPU: Intel UHD 630  
- WIFI/BT: Canon Lake PCH CNVi WiFi
- SMIBIOS iMac19,1
- OpenCore 0.8.4 RELEASE


![11download](https://user-images.githubusercontent.com/7040503/190868987-2ca863c3-1b9b-4d1f-b69e-75f746fb3b90.png)


Tested and found working:
- Boot into MacOS 12.6
- Sleep Wake up from bluetooth mouse or keyboard
- iGPU hardware acceleration
- WIFI and Bluetooth 
- Internal Network Card

Note: USBPorts.kext should be configured on target system to fit desired USB port map. See: Making own USB port map guide below.


Tools used:
- [Opencore](https://dortania.github.io/OpenCore-Install-Guide/) 
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
- [Hackintool](https://github.com/headkaze/Hackintool)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

Guides:
[Custom SSDT's with SSDTTime](https://www.tonymacx86.com/threads/custom-ssdts-using-corpnewts-ssdttime.318976/)
[Making own USB port map](https://www.tonymacx86.com/threads/the-new-beginners-guide-to-usb-port-configuration.286553/#post-2029768)
[How to Map your USB Ports on macOS](https://elitemacx86.com/threads/how-to-map-your-usb-ports-on-macos.581/)
[Intel UHD 630 iGPU configuration](https://www.tonymacx86.com/threads/guide-intel-uhd-graphics-630-coffee-lake-headless-mode-main-card.304000/) for system running only iGPU


