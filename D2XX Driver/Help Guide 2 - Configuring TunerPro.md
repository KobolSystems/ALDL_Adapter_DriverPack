 Configuring ALDL Adapter in TunerPro V5

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
# Install Tuner Pro

## 1. Download TunerPro

- Visit the official TunerPro website: [http://www.tunerpro.net/downloadApp.htm](http://www.tunerpro.net/downloadApp.htm)
- Click on the **Download TunerPro** button.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a12.png?raw=true" style="width: 200px;">

## 2. Run the Installer

- Locate the downloaded file (usually in your **Downloads** folder).
- Double-click the installer (`TunerProSetup.exe`) to begin.

---

## 3. Accept the License Agreement

- Read through the license agreement.
- Click **I Agree** to continue.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a1.png?raw=true" style="width: 200px;">
---

## 4. Start Menu Folder

- Leave it as the default.
- Click **Next**.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a2.png?raw=true" style="width: 200px;">

---

## 5. Additional Tasks

- Leave it as default.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a3.png?raw=true" style="width: 200px;">

---
## 6. Install TunerPro

- Click **Install** to begin the installation.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a4.png?raw=true" style="width: 200px;">
---

## 7. Complete Setup

- Once installation is complete, click **Finish**.
- You can optionally launch TunerPro immediately after installation.
<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a5.png?raw=true" style="width: 200px;">

---

# Verify ALDL Cable Driver Install

You will need the com port number of the ALDL Adapter for Tuner Pro.

*Note this may change from time to time so it is good practice to check it every time you launch the application*

Follow the steps in this document 
[Here](https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/readme.md)

---

# Configure TunerPro

This section will guide you through configuring TunerPro for use with your ALDL Adapter.

---

## 1. Open TunerPro

- Launch **TunerPro** from your desktop or Start Menu.

---

## 2. Access Preferences

- Click on **Tools** in the top menu, then select **Preferences**.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a7.png?raw=true" style="width: 200px;">

---

## 3. Configure Data Acquisition Settings

- In the Preferences window, click on the **Data Acq./Emulation** tab.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a9.png?raw=true" style="width: 200px;">

- Ensure the **Data Acquisition and Logging** section matches the settings shown in the screenshot.

---

## 4. Configure Plug-in Component

- Click on **Configure Plug-in Component** within the same tab.
- Set **Port Type** to **Standard Serial**.
- Set **Port Number** to the COM port assigned to your ALDL Adapter (found via **Device Manager**).

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/a11.png?raw=true" style="width: 200px;">

---

# Important Notes

- **Port Number Display**: If curly brackets `{}` appear around the port number, it means the cable is not properly connected to the computer. Reconnect the cable and restart TunerPro

- **Cable Disconnection**: If the cable is unplugged while TunerPro is running, you must restart the application.

- **Cable Testing**: When testing the cable, ensure it is **unplugged from the vehicle**; otherwise, the test will fail.

