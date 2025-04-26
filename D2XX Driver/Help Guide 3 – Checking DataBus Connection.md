# Help Guide 3 – Checking DataBus Connection Using OSE Enhanced Flash Tool

This guide explains how to verify DataBus connectivity using the **OSE Enhanced Flash Tool** on Windows 10 or 11 systems.

---

## Supported Systems

- **Supported Editions**:
  - Windows 10 Home / Pro / Enterprise / Education (32-bit and 64-bit)
  - Windows 11 Home / Pro / Enterprise / Education (64-bit only)
- **Notes**:
  - Windows 11 32-bit is not supported (Microsoft discontinued 32-bit versions).
  - ARM/ARM64 devices are not supported.

---

## Download OSE Enhanced Flash Tool

- Download the OSE Enhanced Flash Tool from [this link](https://pcmhacking.net/forums/viewtopic.php?t=82).
- Alternatively, an archived copy is available in our repository [here](https://github.com/KobolSystems/ALDL_Adapter_DriverPack/tree/main/D2XX%20Driver/OSE-Enhanced_Flash_Tool).

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b4.png?raw=true" style="width: 250px;">

---

## Open the Tool

1. Double-click the downloaded file to open it.
2. If prompted, install **.NET Framework 3.5**.  
   - This may take some time and requires an active internet connection.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX Driver/Screenshots/b1.png?raw=true" style="width: 250px;">


> **Note**:  
> If you install .NET Framework 3.5, you must **reopen the downloaded file** afterwards.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b12.png?raw=true" style="width: 250px;">


---

## Configure OSE Enhanced Flash Tool

- Click **Options** > **Preferences**.
- Under **Quick Setup**:
  - Set **Logger** to **ALDL Logger**.
  - Set **Interface** to **USB ALDL**.
- Under **Communications Options**:
  - Set **ECM COM Port** to the COM port of your ALDL Adapter (check via Device Manager).
    - Only available/connected COM ports will appear in the dropdown.
  - Set **Baud Rate** to **8192**.
  - Ensure the following options are **unchecked**:
    - Unckeck 'Ignore Echo'
    - Uncheck 'Disable BCM Chatter'
    - Uncheck 'Disable ECM Chatter'
- Click **OK** to save.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b8.png?raw=true" style="width: 250px;">


---

## Testing Step 1 – Check Send and Receive with Loopback

**Setup**:
- Ensure the ALDL Adapter is **unplugged from the vehicle** but **plugged into the laptop**.

**Procedure**:
1. Open **OSE Enhanced Flash Tool**.
2. Verify the correct COM port is selected.
3. In the text box, enter:  
   `F2, 57 01, 00`
4. Click **Auto Calculate Checksum**.
5. Click **Send**.

**Successful Result**:

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b10.png?raw=true" style="width: 250px;">


- A successful response indicates the ALDL Adapter is fully functional.

**Unsuccessful Result**:

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b11.png?raw=true" style="width: 250px;">


- An unsuccessful response generally indicates a **faulty ALDL Adapter**.

---

## Testing Step 2 – Listen to ALDL Data

If "Testing Step 1" was successful, proceed to verify the vehicle's ALDL DataBus:

**Setup**:
- Plug the ALDL Adapter into the vehicle.
- Switch the ignition to **ON** (engine does not need to be running).

**Procedure**:
1. Open **OSE Enhanced Flash Tool**.
2. Verify the correct COM port is selected.
3. Click **Tools** > **Listen to Chatter and Send Custom ALDL Frames**.
4. Click **Listen To Chatter**.

**Expected Result**:

- Within a few seconds, you should see live data frames in the output window.

<img src="https://github.com/KobolSystems/ALDL_Adapter_DriverPack/blob/main/D2XX%20Driver/Screenshots/b9.png?raw=true" style="width: 250px;">

> **Note**:  
> At the time of writing, no vehicle was available for capturing a real-world example.  
> A successful result will display **white text** with messages similar to:  
> `Rx'd Frame = {Actual Data Frame}`

---

