# Intel NUC7i3BNH Changelog

English
- **04-02-2021**

	**Update**
	- Update `SSDT-RTC0.aml`: enabling native `RTC` device only for macOS
	- Add `SSDT-INIT.aml` for initialize `HPTE` (disabling `HPET` device) and `OSYS` variables
	- Add [kext] `IntelMausi` for enabling support for Intel Ethernet (`en2`)
	
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
	- Update `VirtualSMC` v. 1.2.2 beta:
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