# USB to ALDL Adapter - Verifying the Adapter is Installed

## Supported Systems

- This guide is only intended for the following versions of Windows 10/11.
  - Windows 10/11
  - Windows 10/11 Home
  - Windows 10/11 Pro
  - Windows 10/11 Enterprise
  - Windows 10/11 Education
- Windows 10 32 bits and 64 bits are supported.
- Windows 11 64 bits is only supported as Microsoft does not support 32 bits for this OS
- Windows ARM/ARM64 devices are not supported at this time

### Verify Driver Installation

In this step we will check to see if Windows has automatically detected the Adapter and installed the correct driver.
1. Plug in the USB to ALDL Adapter to a USB port on your computer.
2. Right-click on the Windows Start Menu Icon to open the quick access menu.
3. In the quick access menu, click on Device Manager to open it.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/10.png?raw=true" style="width: 200px;">

4. The Device Manager window will open, showing a list of all the devices connected to your computer.
5. Look for "Ports (COM & LPT) if the driver has been automatically installed it will show as "USB Serial Port (COMx) *Where x is the number it has been assigned)
6. if this does not exist, Look for "Other Devices" and if this contains "USB Serial Cable" you will need to manually install the driver pack.

**Driver is Installed**
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/12.png?raw=true" style="width: 600px;">

**Driver is not Installed**
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/11.png?raw=true" style="width: 600px;">
