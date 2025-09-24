# 🪪 Arduino RFID Attendance System

## 📌 Overview
This project uses an **RFID module** with Arduino to log attendance or grant access.  
When a registered RFID card is scanned, the LCD shows **Access Granted**, otherwise **Access Denied**.

---

## 🛠️ Hardware Required
- Arduino Uno/Nano  
- MFRC522 RFID Module  
- RFID Card/Key Fob  
- LCD Display (16x2, I2C)  
- Jumper wires, breadboard  

---

## 🔌 Wiring
- **MFRC522 → Arduino**  
  - SDA → D10  
  - SCK → D13  
  - MOSI → D11  
  - MISO → D12  
  - RST → D9  
  - VCC → 3.3V  
  - GND → GND  

- **LCD (I2C)**  
  - VCC → 5V  
  - GND → GND  
  - SDA → A4  
  - SCL → A5  

---

## ▶️ Usage
1. Install the **MFRC522** library from Arduino IDE Library Manager.  
2. Run the `DumpInfo` example to get your card’s UID.  
3. Replace `allowedUID` in the code with your card UID.  
4. Upload the sketch.  
5. Scan your RFID card → LCD + Serial Monitor shows access result.  

---

## 📂 Repo Structure
