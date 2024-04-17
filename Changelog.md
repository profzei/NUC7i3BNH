# Intel NUC7i3BNH Changelog

English

- **04-17-2024**

	Implemented a cleaner code with various changes.

- **02-19-2023**

	Update to **macOS Big Sur 11.7.4 (20G1120)**

    **Update**
    - Update `OpenCore` v. 0.8.9
    - Update [kext] `AppleALC` v. 1.7.9
    - Update [kext] `HibernationFixup` v. 1.4.8
    - Update [kext] `WhateverGreen` v. 1.6.4

- **02-11-2023**

	Update to **macOS Big Sur 11.7.3 (20G1116)**

	**Update**
	- Update [kext] stripped `AirportItlwm_Big_Sur` v. 2.2.0 beta (commit ddd2768)

- **01-24-2023**

	**OpenCore**
	- Update `config.plist`:
		- Optimized `Intel(R) HD Graphics 620` support editing many entries
		- Added `devide-id` entry for `Intel(R) Sunrise Point-LP High Defintion Audio Controller`

- **01-23-2023**

	Update `Readme` file: added a new section for setting up `BenQ PD2500Q` speakers as default audio output device

- **01-18-2023**

    **Update**
    - Update `OpenCore` v. 0.8.8
    - Update [kext] `AppleALC` v. 1.7.8
    - Update [kext] `Lilu` v. 1.6.3
    - Update [kext] `WhateverGreen` v. 1.6.3
    - Update [driver] `HfsPlus.efi` (commit c2a9898): fix W^X for firmware drivers for ExFAT and HFS+
    - Update [driver] `ExFatDxe.efi` (commit c2a9898): fix W^X for firmware drivers for ExFAT and HFS+

    **OpenCore**
    - Update `config.plist` to support `OpenCore` v. 0.8.8
    - Update for not showing `EFI` partition folder in pickup boot menu since now the magic Acidanthera sequence from OpenCore (v. `0.8.8+`) files is removed (dual boot with Windows is preserved with no issues)

- **01-06-2023**

	**Update**
    - Update `OpenCore` v. 0.8.7
    - Update [kext] `AppleALC` v. 1.7.7
    - Update [kext] `FeatureUnlock` v. 1.1.2
    - Update [kext] `HibernationFixup` v. 1.4.7
    - Update [kext] `RestrictEvents` v. 1.0.9
    - Update [kext] `WhateverGreen` v. 1.6.2
    - Update [kext] stripped `AirportItlwm_Big_Sur` v. 2.2.0 beta (commit e0f745e): some little fixes added to default code
    - Update [kext] stripped `IntelBluetoothFirmware` v. 2.3.0 beta (commit 693f2dc)

    **OpenCore**
    - Update `config.plist` to support `OpenCore` v. 0.8.7

- **10-31-2022**

	Update to **macOS Big Sur 11.7.1 (20G918)**

	**Update**
	- Update [kext] `FakePCIID` v. 1.3.16
	- Update [kext] `FakePCIID_Intel_HDMI_Audio` v. 1.3.16

- **10-06-2022**

	**Update**
	- Update `OpenCore` v. 0.8.5
    - Update [kext] `VoodooPS2Controller` v. 2.3.1
    - Update [kext] stripped `AirportItlwm_Big_Sur` v. 2.2.0 beta (commit ee56708)
    - Update [kext] stripped `AirportItlwm_Catalina` v. 2.2.0 beta (commit ee56708)
    - Added [kext] `FeatureUnlock` v. 1.0.9
    - Added [kext] `USBPorts` with proper mapping for USB Controllers and related active ports (applied some changes in BIOS)

    **OpenCore**
    - No change needed for `config.plist` to support `OpenCore` v. 0.8.5
    - Reduced warning messages number for `Intel(R) HD Graphics 620` in system log during boot phase: they are correct/normal, however eliminating those warnings reduces log-file size thus reducing slightly boot loading time.

- **09-16-2022**

	Update to **macOS Big Sur 11.7 (20G817)**

- **09-11-2022**

	Update to **macOS Big Sur 11.6.8 (20G730)**

	Modified `SMBIOS` to `Macmini8,1`

	**Update**
	- Update `OpenCore` v. 0.8.4
    - Update [kext] `AppleALC` v. 1.7.5
    - Update [kext] `CPUFriend` v. 1.2.6
    - Update [kext] `HibernationFixup` v. 1.4.6
    - Update [kext] `IntelMausi` v. 1.0.7
    - Update [kext] `Lilu` v. 1.6.2
    - Update [kext] `NVMeFix` v. 1.1.0
    - Update [kext] `RestrictEvents` v. 1.0.8
    - Update [kext] `VirtualSMC` + plugins v. 1.3.0
    - Update [kext] `VoodooPS2Controller` v. 2.2.9
    - Update [kext] `WhateverGreen` v. 1.6.1
    - Update [kext] stripped `AirportItlwm_Big_Sur` v. 2.2.0 beta (commit bb86d9f)
    - Update [kext] stripped `AirportItlwm_Catalina` v. 2.2.0 beta (commit bb86d9f)

	**OpenCore**
	- Update `config.plist` to support `OpenCore` v. 0.8.4

- **02-16-2022**

	Updated to **macOS Catalina 10.15.7 (19H1715)** latest Security Update

- **02-02-2022**

	Updated to **macOS Catalina 10.15.7 (19H1713)** latest Security Update

- **12-22-2021**

	Updated BIOS to BNKBL357.86A.0085.2021.0901.1844

- **11-10-2021**

    **Update**
    - Update [kext] stripped `AirportItlwm_Catalina` v. 2.1.0 beta (commit 576b9e1): `iwm` support for LDPC in 11n/11ac mode and better Bluetooth/WiFi coex
    - Update [kext] stripped `IntelBluetoothFirmware` v. 2.1.0 beta (commit a9217e8): updated firmware for Intel Bluetooth 8265 (Build `REL1221` Release version `22.50.0.4`)
    - Update [kext] stripped `IntelBluetoothInjector` v. 2.1.0 beta (commit a9217e8): updated firmware for Intel Bluetooth 8265 (Build `REL1221` Release version `22.50.0.4`)

- **10-31-2021**

	Installed **Security Update 2021-007** for macOS Catalina 10.15.7

	**Update**
	- Update [kext] stripped `AirportItlwm_Catalina` v. 2.1.0 beta (commit 3aab4a6)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 2.0.1
	- Update [kext] stripped `IntelBluetoothInjector` v. 2.0.1

	Update **Safari** v. 15.1

- **09-10-2021**

	**Update**
	- Update `OpenCore` v. 0.7.3
	- Update [kext] `AppleALC` v. 1.6.4
	- Update [kext] `Lilu` v. 1.5.6
    - Update [kext] `HibernationFixup` v. 1.4.3
    - Update [kext] `RestrictEvents` v. 1.0.4
    - Update [kext] `VirtualSMC` + plugins v. 1.2.3
	- Update [kext] `WhateverGreen` v. 1.5.3
	- Update [kext] stripped `AirportItlwm_Catalina` v. 2.1.0 beta (commit 1e857b9)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 2.0.0 beta (commit 06f9d25)
	- Update [kext] stripped `IntelBluetoothInjector` v. 2.0.0 beta (commit 06f9d25)

	**OpenCore**
	- Update `config.plist` to support `OpenCore` v. 0.7.3

	Update to **macOS Catalina 10.15.7 (19H1323)** latest Security Update

- **08-21-2021**

	**Update**
	- Update [kext] stripped `AirportItlwm_Catalina` v. 2.1.0 beta (commit 6bf409c)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 2.0.0 beta (commit dbe8fcc)
	- Update [kext] stripped `IntelBluetoothInjector` v. 2.0.0 beta (commit dbe8fcc)

- **06-27-2021**

	**Update**
	- Revert back to [kext] stripped `IntelBluetoothFirmware` v. 1.1.3 stable (commit 562de1c): Magic Mouse 2 showed some lags with v. 2.0.0 beta (commit beb5224)
	- Revert back to [kext] stripped `IntelBluetoothInjector` v. 1.1.3 stable (commit 562de1c)

- **06-25-2021**

	Apple **Magic Mouse 2** is working wonderfully

	**Update**
	- Update [kext] stripped `AirportItlwm_Catalina` v. 2.0.0 beta (commit 93bf81f)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 2.0.0 beta (commit beb5224)
	- Update [kext] stripped `IntelBluetoothInjector` v. 2.0.0 beta (commit beb5224)

- **05-31-2021**

	**Update**
	- Update [kext] stripped `AirportItlwm_Catalina` v. 2.0.0 beta (commit 4590cd1)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 1.1.3 beta (commit ed27c85)
	- Update [kext] stripped `IntelBluetoothInjector` v. 1.1.3 beta (commit ed27c85)
	- Update `SSDT-PM.aml`: Implemented two different sliders for Display and Device sleeping
	- Add `SSDT-NMVE.aml`

	**OpenCore**
	- Update [driver] `HfsPlus.efi` from latest fw (IM201 and IM161)
	- Update `config.plist`: Improved PCI Devices information coherence

- **05-30-2021**

	**Update**
	- Update `OpenCore` v. 0.6.9
	- Update [kext] `AppleALC` v. 1.6.0
	- Update [kext] `IntelMausi` v. 1.0.6
    - Update [kext] `Lilu` v. 1.5.3
    - Update [kext] `NVMeFix` v. 1.0.7
    - Update [kext] `RestrictEvents` v. 1.0.1
    - Update [kext] `Sinetek-rtsx` v. 9.0
    - Update [kext] `VirtualSMC` + plugins v. 1.2.3
    - Update [kext] stripped `AirportItlwm_Catalina` v. 2.0.0 beta (commit 604a33b)
    - Update [kext] stripped `IntelBluetoothFirmware` v. 1.1.3 beta (commit ed27c85)

    **OpenCore**
    - Update `config.plist` to support `OpenCore` v. 0.6.9

- **05-27-2021**

	**Update**
	- Update `SSDT-VDEV.aml`: removed `PGMM` device for undefined PCI device `0x00080000` (Intel Corporation Core Processor Gaussian Mixture Model)
	- Add `SSDT-IGMM.aml`: 
		- assigned ACPI device name `IGMM` to undefined PCI device `0x00080000` (Intel Corporation Core Processor Gaussian Mixture Model)
		- now `PCI0.IGMM@8` is properly populated in IORegistryExplorer app
		
- **05-26-2021**

	Update **Safari** v. 14.1.1

- **05-05-2021**

	Update **Safari**  Security Patch for WebKit

- **04-28-2021**

	Update to macOS Catalina 10.5.7 Security Update 2021-002 (build 19H1030)
	
	Update **Safari** v. 14.1

	**OpenCore**
	- Update `config.plist`:
		- `Misc -> Debug -> ApplePanic` key set to `true` (previous value was `false`)
		- Removed `-igfxtypec` boot parameter since it determines slow shutdown/reboot
	
	Added a new section in `Readme.md` for making macOS zsh Terminal colorful (therefore improving readability in Terminal.app)
	
- **04-18-2021**

	**Update**
	- Update `SSDT-UIAC.aml`: proper support for `8086:15db` (secondary) USB controller (`SSS1` port)
	
	**OpenCore**
	- Update `config.plist`:
		- Added `-igfxtypec` boot parameter to force DP connectivity for Type-C platforms

- **04-11-2021**

	**Update**
	- Update `SSDT-INIT.aml` for enabling with native approach secondary `XHCI` interface with USB type-C port
	
	Totally fixed issue described [here](https://github.com/profzei/NUC7i3BNH#usb-port-mapping-on-nuc-chassis) for my QHD monitor **BenQ PD2500Q** (resolution: 2048x1152 hiDPI for optimal readability)

- **04-09-2021**

	**Update**
	- Update [kext] `VirtualSMC` + plugins v. 1.2.3 beta (commit 1cb8fd1): fixed fan speed reading
	- Update `SSDT-PM.aml`:
		- Modified structure for `PMCR` device using as Hardware ID `APP9876` as found on iMac18,3
		- Assigned ACPI device name `THRM` to undefined PCI device `0x00140002` (Intel Corporation Thermal Subsystem) in `IODeviceTree` list for enhancing compatibility with thermal zone
	- Update `SSDT-VDEV.aml`:
		- Added `BUS1` device for `SMBUS` Controller (more native or Apple-like approach)
		- Assigned ACPI device name `PGMM` to undefined PCI device `0x00080000` (Intel Corporation Core Processor Gaussian Mixture Model) in `IODeviceTree` list for enhancing compatibility
	
	**OpenCore**
	- Update `config.plist`:
		- Added `compatibility` key for `PciRoot(0x0)/Pci(0x14,0x2)` with value `pci8086,9d21` resulting to vanilla detection for thermal zone (pair with `SSDT-PM.aml` update)
		
- **04-08-2021**

	**Update**
	- Update [kext] stripped `AirportItlwm_Catalina` v. 1.3.0 beta (commit 68bc77c)
	- Update [kext] stripped `IntelBluetoothFirmware` v. 1.1.2 (commit 16bc609)
	- Update `SSDT-EC-USBX.aml`: original `H_EC` device is disabled (through `_STA` method) for not loading `AppleACPIEC.kext`
	- Update `SSDT-PM.aml`: changed returning value for `PMCR._STA` method from `0x0F` to `0x0B`
	- Add `SSDT-FWHD.aml` for enabling Intel 82802 Firmware Hub Device
	
	**OpenCore**
	- Update `config.plist`:
		- Added `H_EC._STA,0,N to H_EC.XSTA,0,N` binary patch (pair with `SSDT-EC-USBX.aml`)
	
- **04-06-2021**

	**Update**
	- Update [kext] `AppleALC` v. 1.5.9
	- Update [kext] `HibernationFixup` v. 1.4.0
	- Update [kext] `Lilu` v. 1.5.2
	- Update [kext] `NVMeFix` v. 1.0.6
	- Update [kext] `VirtualSMC` + plugins v. 1.2.2
	- Update [kext] `WhateverGreen` v. 1.4.9

	**Debug**
	- Update `MaciASL` v. 1.6.0
	
	Since `SMCSuperIO.kext` from official v. 1.2.2 release seems to be [bugged](https://github.com/osy/HaC-Mini/issues/553#issuecomment-814170132) reporting always `0 rpm` for `FAN` sensor, it is replaced with old version taken from previous working beta release

- **04-05-2021**

	Update to macOS Catalina 10.5.7 Supplemental Update + Security Update (build 19H524)
	
	**Update**
	- Add [kext] `HibernationFixup` v. 1.3.9
	
	**OpenCore**
	
	Moving from **Debug** `OpenCore` v. 0.6.7 to **Release** one since system should be stable enough
	- Updated `config.plist`:
		- `Misc -> Debug -> AppleDebug` key set to `false` (previous value was `true`)
		- `Misc -> Debug -> ApplePanic` key set to `false` (previous value was `true`)
		- `Misc -> Debug -> Target` key set to `3` (previous value was `67`)
		- Removed in `NVRAM -> boot-args` key `-v keepsysm=1 debug=0x100` (only needed for debugging purpouses)
	
	Enabling **GUI** for `OpenCanopy` in `config.plist`:
		- `Misc -> Boot -> PickerMode` key set to `External` (previous value was `Builtin`)
		- `Misc -> Boot -> PickerVariant` key set to `Modern` (previous value was `Auto`)
		
- **04-03-2021**

	**Update**
	- Add [kext] `FakePCIID`: atm it's needed for enabling audio over HDMI (it's not a vanilla solution)
	- Add [kext] `FakePCIID_Intel_HDMI_Audio`: atm it's needed for enabling audio over HDMI (it's not a vanilla solution)
	
	**OpenCore**
	- Update `config.plist`:
		- Updated `layout-id` to 45 for Audio device (`PciRoot(0x0)/Pci(0x1f,0x3)`)
		- Proper set-up for supporting `MAT` device:
			- `Booter/Quirks/EnableWriteUnprotector` set to `false` (previous value was `true`)
			- `Booter/Quirks/ProvideCustomSlide` set to `false` (previous value was `true`)
			- `Booter/Quirks/RebuildAppleMemoryMap` set to `true` (previous value was `false`)
			- `Booter/Quirks/SyncRuntimePermissions` set to `true` (previous value was `false`)
		- Added `acpi-wake-type` key for USB 3.0 xHCI Controller (`PciRoot(0x0)/Pci(0x14,0x0)`) for supporting wake-up from keyboard (since it's a desktop I'm not very interested in sleep...)
		- updated config for `PciRoot(0x0)/Pci(0x2,0x0)`:
			- enabled `enable-hdmi-dividers-fix` property
			- enabled `framebuffer-con2-enable` property
			- enabled `framebuffer-con2-has-lspcon` property
			- enabled `framebuffer-con2-preferred-lspcon-mode` property
			- enabled `framebuffer-camellia` property
			- enabled `framebuffer-conX-busid` property
			- enabled `framebuffer-conX-flags` property
			- enabled `framebuffer-conX-index` property
			- enabled `framebuffer-conX-pipe` property
			- enabled `framebuffer-conX-type` property
			- enabled `framebuffer-flags` property
			- enabled `framebuffer-memorycount` property
			- enabled `framebuffer-mobile` property
			- enabled `framebuffer-pipecount` property
			- enabled `framebuffer-portcount` property
		- fixed layout for my keyboard

- **04-02-2021**

	**Update**
	- Update `SSDT-RTC0.aml`: enabling native `RTC` device only for macOS
	- Add `SSDT-INIT.aml` for initialize `HPTE` (disabling `HPET` device) and `OSYS` variables
	- Add [kext] `IntelMausi` v. 1.0.5 for enabling support for Intel Ethernet (`en2`)
	
	**OpenCore**
	- Update `config.plist`:
		- cleaned testing stuff
		- added `PCI0._INI,0,S to XINI,0,S` binary patch
		- added standard `HPET._CRS to XCRS` binary patch
		- forced loading for `com.apple.iokit.IO80211Family` in `Kernel -> Force` section
		- updated config for `PciRoot(0x0)/Pci(0x2,0x0)`:
			- enabled `enable-dpcd-max-link-rate-fix` property
			- enabled `enable-lspcon-support` property
			- enabled `force-online` property
			- enabled `framebuffer-con1-enable` property
			- enabled `framebuffer-con1-has-lspcon` property
			- enabled `framebuffer-con1-preferred-lspcon-mode` property
			- enabled `framebuffer-patch-enable` property
	
	After extensive tests, there is no real benefit on enabling `ALSD`  and `PNLF` devices through `SSDT-ALSD.aml` and `SSDT-PNLF.aml`: I tried since my 2k monitor **BenQ PD2500Q** is equipped with an Ambient Light Sensor.
	
- **04-01-2021**

	**Update**
	- Add [kext] `USBInjectAll` v. 0.7.7
	- Add `SSDT-UIAC.aml` (Thunderbolt Controller not yet included...)
	- Update `SSDT-PM.aml` with proper CPU frequency vector data for Intel 7100U (Low Frequency Mode `LFM` is set @ `08` i.e. **800 MHz** according to [Intel Specifications](https://ark.intel.com/content/www/it/it/ark/products/95442/intel-core-i3-7100u-processor-3m-cache-2-40-ghz.html) while Perf Bias is set @ `01` i.e. default setting for **performance**)
	
	**OpenCore**
	- Update `config.plist`:
		- Added PCI devices properties 
		- Updated `Kernel -> Quirks -> XhciPortLimit` key: now set @ `false` (previous value was `true`) according to new USB config 
	
- **03-31-2021**

	**Update**
	- Update [kext] `VirtualSMC` v. 1.2.2 beta:
		- `SMCSuperIO` supports Embedded Controller sensors for any (atm just one) fan reading in macOS injecting `Intel_EC_V3` value in `ec-device` for `PciRoot(0x0)/Pci(0x1f,0x0)`
	- Update `SSDT-EC-USBX.aml` for implementing Apple EC device and USBX management (modified version from Dortania's one for Desktop machine)
	- Update `SSDT-PM.aml` for proper power management (CPU frequency scaling is still missing)
	- Add `SSDT-SHARE.aml`
	- Add `SSDT-VDEV.aml` adding various virtual devices for macOS compatibility

- **03-30-2021**

	Initial setup for GitHub repo:
	- Update `Changelog`
	- Update `Readme`
		
- **03-29-2021**

	Getting complete **ACPI** dump loading `SysReport` quirk in `config.plist`
	
- **03-21-2021**

	- Update **Safari** to v. 14.0.3
	- Successful (but very rough...) install for **Catalina 10.5.7** (19H2) on Intel NUC7i3BNH