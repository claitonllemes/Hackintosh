[//]: # "Cover Image"

<a><img src="https://user-images.githubusercontent.com/99222756/248500164-c8241be9-6186-48b4-a82d-a2e38aae0006.png" width="100%"></a>

`Hackintosh` é um termo usado para descrever computadores que não são da Apple, mas que rodam o sistema operacional `macOS`. Essas máquinas são configuradas para imitar o hardware da Apple, permitindo que o sistema operacional seja instalado e executado de forma nativa.

<br>

[//]: # "Configuration"

<img src="https://user-images.githubusercontent.com/99222756/248489828-5cb9671d-c873-4742-9e79-6dac500e1516.png" width="100%">

<br>

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Machine:** iMac Retina 5K 27 Inch 2020

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Plataform:** Desktop Intel Core 10Th Gen Comet Lake

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Motherboard:** Gigabyte Z490M Gaming X

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Bios Version:** F21

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Storage:** SSD Samsung 970 EVO Plus 2TB

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **Network:** Fenvi T919 BCM94360 PCIe

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px">**GPU:** Sapphire AMD Radeon RX 6600 8 GB

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **RAM:** 2x16 32gb 3000 Mhz DDR4

<img src="https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg" style="float:left; padding-right:10px"> **SMBios:** iMac20,2

<br>

[//]: # "Bios Setup"

<img src="https://user-images.githubusercontent.com/99222756/248505512-deb5a335-831f-4cda-ac75-2300869c769b.png" width="100%">

<br>

# **Tweaker**

- CPU Upgrade: `Gaming Profile`
- Enhanced Multi-Core Performance: `Enabled`
  ### **Advanced CPU Settings:**
  - Hyper-Threading Technology: `Enabled`
  - VT-d: `Enabled`
- Extreme Memory Profile (X.M.P): `Profile1`

<br>

# **Settings**

### **Plataform Power:**

- Plataform Power Management: `Enabled`
- PCH ASPM: `Enabled`

### **IO Ports:**

- Internal Graphics: `Enabled`
- Above 4G Decoding: `Enabled`
- Re-Size BAR Support: `Disabled`
  ### **Super IO Configuration:**
  - Serial Port: `Enabled`
  ### **USB Configuration:**
  - XHCI Hand-off: `Enabled`
  ### **SATA And RST Configuration:**
  - SATA Mode Selection: `AHCI`

### **Miscellaneous:**

- Intel Plataform Trust Technology (PPT): `Enabled`
  ### **Trust Computing:**
  - Security Device Support: `Enabled`

<br>

# **Boot**

- CFG Lock: `Disabled`
- Security Option: `System`
- Full Screen Logo Show: `Disabled`
- Fast Boot: `Enabled`
- CSM Support: `Disabled`
  ### **Secure Boot:**
  - Secure Boot Enable: `Enabled`
  - Secure Boot Mode: `Standard`

<br>

[//]: # "USB Mapping"

<img src="https://user-images.githubusercontent.com/99222756/248507670-4048db21-eeba-4cec-924f-15946a4408fc.png" width="100%">

<br>

# **Internal**

<br>

|                                                      Status                                                       |  Connector   | Type | Port | Code | Description       |
| :---------------------------------------------------------------------------------------------------------------: | :----------: | :--: | :--: | :--: | :---------------- |
| <img src="https://user-images.githubusercontent.com/99222756/248509879-7473ad54-d417-4ac0-b364-517eaf0936e1.svg"> | **Internal** | XHCI | HS10 | 255  | _Fenvi Wifi Card_ |
| <img src="https://user-images.githubusercontent.com/99222756/248509881-dfd36b1b-5f74-43fd-9ee1-15d3ea39ffc4.svg"> | **Internal** | XHCI | HS13 | 255  | _RGB Control_     |

<br>

# **USB 2.0**

<br>

|                                                      Status                                                       |  Connector   | Type | Port | Code | Description       |
| :---------------------------------------------------------------------------------------------------------------: | :----------: | :--: | :--: | :--: | :---------------- |
| <img src="https://user-images.githubusercontent.com/99222756/248509879-7473ad54-d417-4ac0-b364-517eaf0936e1.svg"> | **Internal** | XHCI | HS10 | 255  | _Fenvi Wifi Card_ |
| <img src="https://user-images.githubusercontent.com/99222756/248509881-dfd36b1b-5f74-43fd-9ee1-15d3ea39ffc4.svg"> | **Internal** | XHCI | HS13 | 255  | _RGB Control_     |

[//]: # "Credits"

<img src="https://user-images.githubusercontent.com/99222756/248505509-95952bff-79ea-4936-9886-b6620d832e2e.png" width="100%">

**Thank you all for the excellent work and dedication on this amazing project**

- ##### **Thanks to** [@acidanthera](https://github.com/acidanthera) for:

  - ###### [Opencore](https://github.com/acidanthera/OpenCorePkg) _OpenCore bootloader with development SDK_

- ##### **Thanks to** [@corpnewt](https://github.com/corpnewt) for:

  - ###### [ProperTree](https://github.com/corpnewt/ProperTree) _A cross-platform GUI plist editor written using Python_
  - ###### [SSDTTime](https://github.com/corpnewt/SSDTTime) _A simple tool designed to make creating SSDTs simple. Supports macOS, Linux and Windows_
  - ###### [USBMap](https://github.com/corpnewt/USBMap) _Python script for mapping USB ports in macOS and creating a custom injector kext_
  - ###### [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) _Python script that uses acidanthera's macserial to generate SMBIOS and optionally saves them to a plist_
  - ###### [GibMacOS](https://github.com/corpnewt/gibMacOS) _Script that can download macOS components direct from Apple_
  - ###### [MountEFI](https://github.com/corpnewt/MountEFI) _Automatic mount EFI Script_
  - ###### [OCconfigcompare](https://github.com/corpnewt/OCConfigCompare) _Python script to compare two plists and list missing keys in either_

- ##### **Thanks to** [@luchina-gabriel](https://github.com/luchina-gabriel) for:

  - ###### [Mcrecovery](https://github.com/luchina-gabriel/macrecovery) _Tool that helps to automate recovery interaction_
  - ###### [Base EFI 10Th Gen](https://github.com/luchina-gabriel/BASE-EFI-INTEL-DESKTOP-10THGEN-COMET-LAKE) _Base EFI Intel for Comet Lake_
