<img src="https://user-images.githubusercontent.com/99222756/248500164-c8241be9-6186-48b4-a82d-a2e38aae0006.png" width="100%">

`Hackintosh` is a term used to describe non-Apple computers that run the `macOS` operating system. These machines are configured to mimic Apple hardware, allowing the operating system to install and run natively.

---

<br>

![Configuration](https://user-images.githubusercontent.com/99222756/248489828-5cb9671d-c873-4742-9e79-6dac500e1516.png "Configuration")

<details><summary>Basic information about the platform used to create the EFI. Hardware based on x86 Intel Comet Lake architecture of 10th Generation. Open for more information</summary><br>

<br>

| **Build**  | **Info**     | **Description**                       |
| :--------: | :----------- | :------------------------------------ |
| ![][Check] | Machine      | iMac Retina 5K 27 Inch 2020           |
| ![][Check] | Plataform    | Intel Core 10Th Gen Comet Lake        |
| ![][Check] | Motherboard  | Gigabyte Z490M Gaming X               |
| ![][Check] | Bios Version | F21                                   |
| ![][Check] | Storage      | iMac SSD Samsung 970 EVO Plus 2TB     |
| ![][Check] | Network      | iMac Fenvi T919 BCM94360 PCIe         |
| ![][Check] | GPU          | iMac Sapphire AMD Radeon RX 6600 8 GB |
| ![][Check] | RAM          | 2x16 32gb 3000 Mhz DDR4               |
| ![][Check] | SMBios       | iMac20,2                              |

</details>

<br>

![Bios Setup](https://user-images.githubusercontent.com/99222756/248505512-deb5a335-831f-4cda-ac75-2300869c769b.png "Bios Setup")

**<details><summary>Open Details</summary><br>**

# **Tweaker**

<br>

- CPU Upgrade: `Gaming Profile`
- Enhanced Multi-Core Performance: `Enabled`
  ### **Advanced CPU Settings:**
  - Hyper-Threading Technology: `Enabled`
  - VT-d: `Enabled`
- Extreme Memory Profile (X.M.P): `Profile1`

# **Settings**

<br>

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

# **Boot**

<br>

- CFG Lock: `Disabled`
- Security Option: `System`
- Full Screen Logo Show: `Disabled`
- Fast Boot: `Enabled`
- CSM Support: `Disabled`
  ### **Secure Boot:**
  - Secure Boot Enable: `Enabled`
  - Secure Boot Mode: `Standard`

<br>

</details> <br>

![USB Mapping](https://user-images.githubusercontent.com/99222756/248507670-4048db21-eeba-4cec-924f-15946a4408fc.png "USB Mapping")

**<details><summary>Open Details</summary><br>**

So the process of USB mapping is defining your ports to macOS and telling it what kind they are, the reasons we want to do this are:

<br>

- macOS is very bad at guessing what kind of ports you have
- Some ports may run below their rated speed
- Some ports may outright not work
- Bluetooth not working
- Certain services like Handoff may not work correctly
- Sleep may break
- Broken Hot-Plug
- Even data corruption from `XhciPortLimit`

You don't have to worry about any of this, as I've already done all the heavy lifting. But if you want to go deeper into this subject, you can access the official port mapping guide from the OpenCore team

<br>

![USB Mapping Ports](https://user-images.githubusercontent.com/99222756/249294437-f612cb9f-d29a-4dbe-bf57-21f08f25f062.png "USB Mapping Ports")

<br>

| **Status** | **Connector** | **Type** | **Port** | **Code** | **Description**   |
| :--------: | :-----------: | :------: | :------: | :------: | :---------------- |
|  ![][on]   |   Internal    |   XHC    |   HS10   |   255    | Fenvi Wifi Card   |
|  ![][off]  |   Internal    |   XHC    |   HS13   |   255    | RGB Control       |
|  ![][on]   |    USB 2.0    |   XHC    |   HS01   |    0     | Port 04 Red       |
|  ![][on]   |    USB 2.0    |   XHC    |   HS03   |    0     | Port 01 Blue      |
|  ![][off]  |    USB 2.0    |   XHC    |   HS04   |    0     | Port 02 Blue      |
|  ![][on]   |    USB 2.0    |   XHC    |   HS05   |    0     | Port 05 White     |
|  ![][on]   |    USB 2.0    |   XHC    |   HS06   |    0     | Port 06 Blue      |
|  ![][on]   |    USB 2.0    |   XHC    |   HS07   |    0     | Front Panel Blue  |
|  ![][on]   |    USB 2.0    |   XHC    |   HS11   |    0     | Front Panel Black |
|  ![][on]   |    USB 2.0    |   XHC    |   HS12   |    0     | Front Panel Black |
|  ![][on]   |    USB 3.0    |   XHC    |   SS17   |    3     | Port 04 Red       |
|  ![][on]   |    USB 3.0    |   XHC    |   SS19   |    3     | Port 01 Blue      |
|  ![][on]   |    USB 3.0    |   XHC    |   SS20   |    3     | Port 02 Blue      |
|  ![][on]   |    USB 3.0    |   XHC    |   SS21   |    3     | Port 05 White     |
|  ![][on]   |    USB 3.0    |   XHC    |   SS22   |    3     | Port 06 Blue      |
|  ![][on]   |    USB 3.0    |   XHC    |   SS23   |    3     | Front Panel Blue  |
|  ![][off]  |   USBC 2.0    |   XHC    |   HS02   |    8     | Port 03           |
|  ![][on]   |   USBC 3.0    |   XHC    |   SS18   |    9     | Port 03           |

<br>

</details> <br>

![Utilities and Tools](https://user-images.githubusercontent.com/99222756/250302428-cab44bc3-fb85-44e5-a13d-5c68ee2b7793.png "Utilities and Tools")

**<details><summary>Open Details</summary><br>**

A set of tools that help a lot in creating your EFI. These tools often facilitate and automate complex tasks for those who don't want to do it manually.

<br>

|                       Download                        | Tool       | Description                                                                                             |
| :---------------------------------------------------: | :--------- | :------------------------------------------------------------------------------------------------------ |
| [![download]](https://github.com/corpnewt/ProperTree) | ProperTree | A cross-platform GUI plist editor written using Python                                                  |
|  [![download]](https://github.com/corpnewt/SSDTTime)  | SSDTTime   | A simple tool designed to make creating SSDTs simple. Supports macOS, Linux and Windows                 |
|   [![download]](https://github.com/corpnewt/USBMap)   | USBMap     | Python script for mapping USB ports in macOS and creating a custom injector kext                        |
| [![download]](https://github.com/corpnewt/GenSMBIOS)  | GenSMBIOS  | Python script that uses acidanthera's macserial to generate SMBIOS and optionally saves them to a plist |
|  [![download]](https://github.com/corpnewt/MountEFI)  | MountEFI   | Automatic mount EFI Script                                                                              |

##### **Copyright ©** [@corpnewt](https://github.com/corpnewt)

<br>

|                                          Download                                           | Tool              | Description                   |
| :-----------------------------------------------------------------------------------------: | :---------------- | :---------------------------- |
| [![download]](https://github.com/luchina-gabriel/BASE-EFI-INTEL-DESKTOP-10THGEN-COMET-LAKE) | Base EFI 10Th Gen | Base EFI Intel for Comet Lake |

##### **Copyright ©** [@luchina-gabriel](https://github.com/luchina-gabriel)

</details> <br>

![Special Thanks](https://user-images.githubusercontent.com/99222756/248505509-95952bff-79ea-4936-9886-b6620d832e2e.png "Special Thanks")

**<details open><summary>Thank you all for the excellent work and dedication on this amazing project</summary>**

<br>

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

</details>

[Check]: https://user-images.githubusercontent.com/99222756/248503004-7349ffa2-4e69-4269-82ee-ea4a6610bf77.svg
[off]: https://user-images.githubusercontent.com/99222756/248509881-dfd36b1b-5f74-43fd-9ee1-15d3ea39ffc4.svg
[on]: https://user-images.githubusercontent.com/99222756/248509879-7473ad54-d417-4ac0-b364-517eaf0936e1.svg
[download]: https://user-images.githubusercontent.com/99222756/250302803-118b94fd-9732-4eaf-b7db-e6a54df58609.svg
