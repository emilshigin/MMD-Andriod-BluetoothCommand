# Android-BLECommand

This project showcases an internal Android tool developed for **Micro Medical Devices (MMD)** to enable wireless communication between Android systems and Arduino-based hardware.  
It allows engineers and technicians to send configuration commands, test responses, and automate calibration steps over Bluetooth — used for **R&D of new product prototypes**.

### Demo
<img src="https://github.com/emilshigin/MMD-Andriod-BluetoothCommand/blob/main/RetinalCamera-Demo-Editoptimize.gif?raw=true" alt="Demo of device pairing between Android phone and Arduino, wirelessly controlled to send data and make an LED flash" width="600">

---

### Overview
- **Purpose:** Streamline hardware calibration and command testing via a mobile interface.  
- **Functionality:** Scans for nearby Arduino BLE devices, pairs and connects, and sends commands.  
- **Outcome:** Reduced manual testing time during early-stage device prototyping and validation.

---

### My Contributions
- Designed and developed the **Android BLE communication layer** (Java / Kotlin).  
- Updated Arduino firmware to support **Bluetooth Low Energy (BLE)** communication.  
- Created the **UI and interaction logic** for device discovery, pairing, and command transmission.  
- Implemented **data persistence** for command presets and automated reconnection to known devices.  
- Collaborated with R&D hardware engineers to validate the protocol and ensure reliable device communication.

---

### Built With
- **Android Studio** (Java / Kotlin)  
- **Arduino Nano 33 BLE Rev2**  
- **Bluetooth Low Energy (BLE)** Protocol  
- **Android BLE APIs**

---

### Credits
- **Android App:** Emil D. Shigin  
- **Arduino BLE Code:** Emil D. Shigin  
- **Base Arduino Code:** R&D Team  
- **Circuit Design:** R&D Team  

---

### Step-by-Step
1. Open the app.  
2. Press **“Device Scan”** to search for Arduino devices currently powered on and running the companion Arduino code.  
   - If Bluetooth is disabled, a prompt will appear asking to enable it.  
3. Select the Arduino device from the list.  
   - A pairing popup will appear. Once paired, the app will auto-reconnect to this device on future launches.  
   - The “Connected Device” status will update to the Arduino device name.  
4. Press any command button to send it to the Arduino.  
5. To send a custom command, type it into the text field and press **“Send Data.”**  
6. Press and hold any button to save it as a preset. Presets are stored until the app is uninstalled.

---

⚠️ *This repository contains internal project documentation and demonstration media for professional portfolio purposes only.  
All proprietary source code remains the property of Micro Medical Devices.*
