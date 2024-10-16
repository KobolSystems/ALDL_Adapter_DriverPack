# USB to ALDL Adapter Driver Install Guide
## FTDI FT230X

### Important Note.
When you plug in the FT230X USB-to-Serial adapter, Windows should automatically detect it and install the correct drivers for it. 
In most cases, no additional setup is necessary. However, if Windows fails to install the correct drivers or if the adapter isn't recognized, follow the steps below to manually install the driver. 

### Introduction
The purpose of this application note is to provide users of FTDI chips with a simple procedure for installing FTDI drivers for their devices under Windows 10 and Windows 11 as both OS versions
are similar.

- This installation guide is only intended for installing FTDI devices on the following versions of Windows 10/11.
  - Windows 10/11
  - Windows 10/11 Home
  - Windows 10/11 Pro
  - Windows 10/11 Enterprise
  - Windows 10/11 Education
- Windows 10 32 bits and 64 bits are supported.
- Windows 11 64 bits is only supported as Microsoft does not support 32 bits for this OS
- Windows ARM/ARM64 devices are not supported at this time
- Linux and MacOS devices require different drivers

### Check for Plug and Play Installation
In this step we will check to see if Windows has automatically detected the Adapter and installed the correct driver.

1. Plug in the USB to ALDL Adapter to a USB port on your computer.
2. Right-click on the Windows Start Menu Icon to open the quick access menu.
3. In the quick access menu, click on Device Manager to open it.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/10.png?raw=true" style="width: 200px;">

4. The Device Manager window will open, showing a list of all the devices connected to your computer.
5. Look for "Ports (COM & LPT) if the driver has been automatically installed it will show as "USB Serial Port (COMx) *Where x is the number it has been assigned)
6. if this does not exist, Look for "Other Devices" and if this contains "USB Serial Cable" you will need to manually install the driver pack.

**Driver is not Installed**

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/11.png?raw=true" style="width: 600px;">

<br><br>
**Driver is Installed**

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/12.png?raw=true" style="width: 600px;">



### Manual Driver Installation

1. download and extract the "CDM212364_Setup.zip" from this repository.
2. navigate to the folder where you extracted the driver setup.exe and right-click and select "Run as administrator".
3. You may see a message from ‘User Access Control’ asking "Do you want to allow this app to make changes to your PC?." If so, click Yes to continue
4. Press the Extract button as shown in Figure below
   (Insert screenshot here)

5. Follow the installation instructions shown in Figure below including license terms agreement acceptance
6. Follow the "Check for Plug and Play Installation" steps to verifiy driver installation and to obtain the COM port number (this may be needed by your Diagnostic Software).



1. Download the CDM212364_Setup.zip file from this repository and extract it to a convenient location on your computer.
2. Navigate to the folder where you extracted the setup files, locate setup.exe, right-click on it, and select Run as administrator.
3. If prompted by User Account Control with the message, "Do you want to allow this app to make changes to your PC?", click Yes to continue.
4. Press the Extract button as shown in the screenshot below.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/1.png?raw=true" style="width: 400px;">
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/2.png?raw=true" style="width: 400px;">

5. Follow the installation instructions, including accepting the license terms, as shown in the screenshot below.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/3.png?raw=true" style="width: 400px;">

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/4.png?raw=true" style="width: 400px;">

6. Verify Installation
Complete the "Check for Plug and Play Installation" steps to verify the driver installation and obtain the COM port number, which may be required by your diagnostic software.



**Note:** The device must be physically plugged in after running the setup exe to complete the
installation.
