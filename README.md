Absolutely. Below is the **complete `README.md` code**, from the exact project title through the license section, with a clean GitHub design and only the required information.

```markdown
# 🏠 Mobile-Controlled Home Automation System

<p align="center">
  <img src="images/1.jpg" alt="Mobile-Controlled Home Automation System" width="750">
</p>

<p align="center">
  <b>Arduino Nano • HC-05 Bluetooth • PIR Sensor • 4-Channel Relay</b>
</p>

---

## 📌 Project Overview

The **Mobile-Controlled Home Automation System** is an embedded home automation project designed to control electrical appliances wirelessly using a **mobile phone and Bluetooth communication**.

The system uses an **Arduino Nano** as the main controller, an **HC-05 Bluetooth module** for wireless communication, a **PIR motion sensor** for motion detection, and a **4-channel relay module** for controlling appliances such as a lamp and fan.

The project demonstrates the integration of **microcontrollers, wireless communication, sensors, and relay-based control** in a practical home automation application.

---

## ✨ Features

- 📱 Mobile-based appliance control
- 🔵 Bluetooth communication using HC-05
- ⚙️ Arduino Nano based control
- 💡 Lamp ON/OFF control
- 🌀 Fan ON/OFF control
- 🚨 PIR-based motion detection
- 🔌 4-channel relay for multiple appliances
- 🏠 Expandable home automation system

---

## 🧩 Hardware Components

| Component | Purpose |
|---|---|
| **Arduino Nano** | Main microcontroller |
| **HC-05 Bluetooth Module** | Wireless communication with mobile |
| **PIR Motion Sensor** | Motion detection |
| **4-Channel Relay Module** | Appliance switching |
| **Lamp** | Controlled appliance |
| **Fan** | Controlled appliance |
| **AC/DC Power Supply** | Provides required power |
| **Switch/Socket Board** | Appliance connection |
| **Jumper Wires** | Circuit connections |

---

## 🔧 System Architecture

```text
                ┌──────────────────────┐
                │     Mobile Phone     │
                │   Control Interface  │
                └──────────┬───────────┘
                           │
                      Bluetooth
                           │
                           ▼
                   ┌───────────────┐
                   │     HC-05     │
                   │   Bluetooth   │
                   └───────┬───────┘
                           │
                          UART
                           │
                           ▼
                   ┌───────────────┐
                   │  Arduino Nano │
                   │ Main Controller│
                   └───────┬───────┘
                           │
              ┌────────────┴────────────┐
              │                         │
              ▼                         ▼
       ┌─────────────┐          ┌──────────────┐
       │ PIR Sensor  │          │ 4-CH Relay   │
       │   Motion    │          │    Module    │
       └─────────────┘          └──────┬───────┘
                                       │
                              ┌────────┼────────┐
                              ▼        ▼        ▼
                            Lamp      Fan    Other Loads
```

---

## 🔄 Working Principle

1. The user sends a control command from a **mobile phone**.
2. The command is transmitted wirelessly through **Bluetooth**.
3. The **HC-05 Bluetooth module** receives the command.
4. The HC-05 sends the received data to the **Arduino Nano through UART**.
5. The Arduino Nano processes the command.
6. The corresponding relay channel is activated or deactivated.
7. The relay switches the connected appliance.
8. The **PIR sensor** detects motion and provides an additional input for automation logic.

### Control Flow

```text
Mobile Phone
     ↓
 Bluetooth
     ↓
   HC-05
     ↓
   UART
     ↓
Arduino Nano
     ↓
Relay Module
     ↓
Appliance
```

---

## 📱 Mobile Control

The appliances can be controlled from a Bluetooth-enabled mobile application.

Example commands:

```text
LIGHT_ON
LIGHT_OFF

FAN_ON
FAN_OFF
```

The exact command format depends on the mobile application and Arduino firmware used in the project.

---

## 🚨 PIR Motion Detection

The PIR sensor detects human movement in the monitored area.

```text
Motion Detected
       ↓
 Arduino Reads PIR
       ↓
 Automation Logic
       ↓
 Required Action
```

The PIR sensor can be used for automatic lighting, occupancy detection, or future security-related features.

---

## 🔌 Relay Control

The 4-channel relay module allows multiple electrical loads to be controlled independently.

| Relay Channel | Example Load |
|---|---|
| **CH1** | Lamp |
| **CH2** | Fan |
| **CH3** | Additional Appliance |
| **CH4** | Additional Appliance |

The unused relay channels can be used to expand the system with additional appliances.

---

## 📡 Communication

### HC-05 ↔ Arduino Nano

The HC-05 communicates with the Arduino Nano using **UART/serial communication**.

```text
Mobile Phone
     │
 Bluetooth
     │
     ▼
   HC-05
     │
    UART
     │
     ▼
Arduino Nano
```

---

## 🛠️ Technologies Used

- **Arduino Nano**
- **Embedded C/C++**
- **HC-05 Bluetooth**
- **UART / Serial Communication**
- **PIR Motion Sensor**
- **4-Channel Relay Module**
- **Microcontroller Programming**
- **Home Automation**

---

## 🧠 Engineering Concepts

This project demonstrates practical implementation of:

- Microcontroller programming
- GPIO interfacing
- UART communication
- Bluetooth communication
- Sensor interfacing
- Relay and actuator control
- Wireless appliance control
- Hardware-software integration
- Embedded automation

---

## 📁 Repository Structure

```text
Mobile-Controlled-Home-Automation/
│
├── README.md
│
├── src/
│   └── home_automation.ino
│
├── images/
│   └── 1.jpg
│
├── hardware/
│   └── circuit_diagram.png
│
└── LICENSE
```

---

## 🚀 Getting Started

### 1. Hardware Setup

Connect the following components to the Arduino Nano:

- HC-05 Bluetooth module
- PIR motion sensor
- 4-channel relay module
- Required power supply and peripherals

Connect the relay outputs to the demonstration appliances according to the circuit design.

### 2. Upload the Firmware

1. Open the Arduino firmware in **Arduino IDE**.
2. Configure the Bluetooth serial interface.
3. Configure the PIR sensor input pin.
4. Configure the relay output pins.
5. Configure the supported mobile commands.
6. Upload the firmware to the Arduino Nano.

### 3. Connect the Mobile Device

1. Power on the system.
2. Pair the mobile phone with the **HC-05 Bluetooth module**.
3. Open the Bluetooth control application.
4. Send the required command.
5. Observe the corresponding relay and appliance response.

---

## 📊 Project Specifications

| Parameter | Details |
|---|---|
| **Project Type** | Embedded Home Automation |
| **Main Controller** | Arduino Nano |
| **Wireless Module** | HC-05 Bluetooth |
| **Control Device** | Mobile Phone |
| **Sensor** | PIR Motion Sensor |
| **Actuator Interface** | 4-Channel Relay |
| **Communication** | Bluetooth / UART |
| **Controlled Appliances** | Lamp, Fan & Expandable Loads |

---

## 🎥 Project Demonstration

### YouTube Demo

[▶️ Watch the Project Demonstration](https://youtu.be/iD15hAr4c-Q?si=9zd7apeNmU71yhbH)

---

## 🔮 Future Enhancements

The system can be further enhanced with:

- Wi-Fi-based remote control
- ESP32-based implementation
- Web or mobile dashboard
- Energy monitoring
- Automatic lighting
- Scheduling and timers
- Temperature and humidity monitoring
- Smart energy-saving features
- Home security notifications

---

## 🎓 Learning Outcomes

This project provided practical experience in:

- Arduino programming
- Embedded C/C++
- Bluetooth communication
- UART protocol
- Sensor interfacing
- Relay control
- Wireless device control
- Hardware troubleshooting
- Embedded system integration

---

## ⚠️ Safety Notice

This project may involve controlling **mains-powered electrical appliances**.

> ⚠️ **Do not work directly with 220/230 V AC wiring unless proper electrical isolation, protection, enclosure, and qualified supervision are available.**

The low-voltage Arduino and Bluetooth circuitry should remain properly isolated from hazardous mains voltage.

---

## 📄 License

This project is developed for **educational and demonstration purposes**.

You may use and modify the project for learning and academic purposes with appropriate attribution.

---

## 👨‍💻 Author

### **Anupam Jadhav**

**Electronics & Telecommunication Engineering**  
**K.K. Wagh Institute of Engineering Education & Research, Nashik**

**Interests:**  
`Embedded Systems` · `IoT` · `Microcontrollers` · `Automation` · `Electronics`

---

⭐ **If you find this project useful, consider giving the repository a star!**
```
