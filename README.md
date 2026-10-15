# Health Monitoring System Using MAX30102

An embedded health monitoring system based on the **LPC2148 ARM7 microcontroller** that measures heart rate and estimates blood oxygen saturation (SpO₂) using the MAX30102 sensor. The project demonstrates sensor interfacing, I²C communication, Embedded C programming, and optional IoT-based remote monitoring.

## 📌 Project Overview

The **Health Monitoring System** integrates the MAX30102 optical sensor with the LPC2148 microcontroller to collect red and infrared sensor readings. The firmware processes these readings to estimate heart rate and SpO₂.

The system can display measurements on an LCD and transmit data to an IoT platform through an ESP-01 Wi-Fi module when those features are implemented.

## 📋 Project Details

| Category | Details |
|---|---|
| **Project Title** | Health Monitoring System Using MAX30102 |
| **Project Type** | Embedded Systems / IoT |
| **Microcontroller** | LPC2148 ARM7 |
| **Programming Language** | Embedded C |
| **Sensor** | MAX30102 |
| **Communication Protocol** | I²C |
| **Wireless Module** | ESP-01 Wi-Fi |
| **IoT Platform** | ThingSpeak |
| **Development Environment** | Keil µVision |
| **Programming Tool** | Flash Magic |

## 🎯 Objectives

- Measure heart rate using the MAX30102 sensor.
- Estimate blood oxygen saturation (SpO₂).
- Interface the MAX30102 with the LPC2148 using I²C.
- Process sensor readings using Embedded C.
- Display measurements on an LCD, if configured.
- Support remote monitoring through ESP-01 and ThingSpeak, if implemented.
- Demonstrate embedded firmware development and hardware–software interfacing.

## ⚙️ Key Features

- **Heart Rate Monitoring:** Uses optical sensor readings to estimate heart rate.
- **SpO₂ Estimation:** Processes red and infrared readings to estimate blood oxygen saturation.
- **I²C Communication:** Enables communication between the MAX30102 and LPC2148.
- **Embedded C Firmware:** Handles sensor configuration, data acquisition, and processing.
- **LCD Display:** Displays measurements and system status when configured.
- **IoT Integration:** Supports remote data visualization when wireless connectivity is implemented.

## 🧰 Hardware Components

| Component | Purpose |
|---|---|
| **LPC2148 ARM7 MCU** | Main controller |
| **MAX30102 Sensor** | Heart rate and SpO₂ sensing |
| **ESP-01 Wi-Fi Module** | Wireless transmission, if implemented |
| **16×2 LCD** | Displays measurements, if connected |
| **Power Supply** | Supplies power to the circuit |
| **Connecting Wires** | Hardware interconnections |

## 💻 Software & Technologies

- **Embedded C**
- **ARM7 / LPC2148**
- **Keil µVision**
- **Flash Magic**
- **I²C Communication**
- **UART Communication**
- **Sensor Interfacing**
- **Firmware Development and Debugging**
- **ThingSpeak IoT Integration**, if implemented

## 🔌 Peripheral Interfaces

### MAX30102 Sensor – I²C

The MAX30102 communicates with the LPC2148 through the **I²C protocol**.

- **7-bit I²C Address:** `0x57`
- **Interface:** I²C
- **Purpose:** Collects red and infrared optical sensor readings.

The firmware processes the collected readings to estimate heart rate and SpO₂.

### ESP-01 – UART and Wi-Fi

The ESP-01 can communicate with the LPC2148 through UART and transmit measurements over Wi-Fi to an IoT platform such as ThingSpeak.

### LCD Display

A 16×2 LCD can display heart rate, estimated SpO₂, and system status when the LCD interface is configured.

## 🏗️ System Architecture

The LPC2148 acts as the central controller and communicates with the MAX30102 sensor through I²C. Processed measurements can be displayed on an LCD or transmitted wirelessly through ESP-01 when implemented.

### System Block Diagram

![Health Monitoring System Block Diagram](system_block_diagram.jpg)

*The block diagram illustrates the system architecture and the connections between the microcontroller and peripherals. Optional LCD and IoT features depend on the implemented hardware and firmware.*

**System flow:**

MAX30102 Sensor → I²C → LPC2148 ARM7 → LCD Display / ESP-01 → ThingSpeak

## 🔄 System Working

### 1. System Initialization

The LPC2148 initializes the required GPIO pins, I²C interface, and other configured peripherals.

### 2. Sensor Initialization

The firmware configures the MAX30102 sensor for red and infrared optical data collection.

### 3. Data Acquisition

The sensor collects optical readings, which are transferred to the microcontroller through I²C.

### 4. Heart Rate and SpO₂ Estimation

The firmware processes the collected sensor readings to estimate heart rate and blood oxygen saturation.

### 5. Display of Measurements

The measured or estimated values can be displayed on an LCD, depending on the implemented hardware.

### 6. IoT Monitoring

If the ESP-01 and ThingSpeak features are implemented, the measurements can be transmitted over Wi-Fi for remote visualization.

## 📷 Project Images

### 🔬 Health Monitoring System Setup

The hardware setup of the Health Monitoring System using the LPC2148 ARM7 microcontroller and MAX30102 sensor.

![Health Monitoring System Setup](health_monitoring_setup_1.jpg)

### 🩺 MAX30102 Sensor Setup

A view of the MAX30102 sensor and its hardware connections used for health monitoring.

![MAX30102 Sensor Setup](health_monitoring_setup_2.jpg)

## 📁 Project Structure

The repository contains Embedded C source code, startup files, header files, project documentation, and images.

```text
Health-Monitoring-System-Using-MAX30102/
│
├── MAX.c
├── Startup.d
├── Startup.lst
├── Startup.o
├── Startup.s
├── Timer1.c
├── all_defines.h
├── delay.c
├── delay.crf
├── delay.d
├── README.md
├── system_block_diagram.jpg
├── health_monitoring_setup_1.jpg
└── health_monitoring_setup_2.jpg
```

*This is an illustrative structure based on the visible repository files. Keep any additional existing files and folders in your actual repository.*

## 🧠 Concepts Demonstrated

This project demonstrates practical experience with:

- Embedded C programming
- ARM7 architecture
- LPC2148 microcontroller programming
- I²C communication
- MAX30102 sensor interfacing
- Heart rate and SpO₂ estimation
- UART communication
- Peripheral interfacing
- Firmware development and debugging
- Hardware–software integration
- IoT data transmission, if implemented

## 🚀 Future Enhancements

Possible improvements include:

- Adding real-time health data logging.
- Improving signal filtering and measurement processing.
- Adding configurable alerts for selected thresholds.
- Building a web or mobile dashboard for remote monitoring.
- Storing historical readings for later analysis.
- Improving wireless connectivity and cloud-upload reliability.

## 👩‍💻 Author

**Pulakanti Sai Niharika**

**B.Tech – Electronics and Communication Engineering (ECE)**

GitHub: [P-SAI-NIHARIKA](https://github.com/P-SAI-NIHARIKA)

## 📌 Project Information

- **Project:** Health Monitoring System Using MAX30102
- **Project Type:** Embedded Systems / IoT
- **Controller:** LPC2148 ARM7
- **Programming Language:** Embedded C
- **Sensor:** MAX30102
- **Domain:** Embedded Systems

---

⭐ **This project demonstrates practical implementation of an embedded system by interfacing a biomedical sensor with the LPC2148 ARM7 microcontroller.**

**Disclaimer:** This project is intended for educational purposes. Sensor-derived readings are not a substitute for medical-grade measurements or professional medical advice.

# Health Monitoring System Using MAX30102

An embedded health monitoring system based on the LPC2148 ARM7 microcontroller that measures heart rate and estimates blood oxygen saturation (SpO₂) using the MAX30102 sensor. The project demonstrates sensor interfacing, I²C communication, Embedded C programming, and optional IoT-based remote monitoring.

## 📌 Project Overview

The Health Monitoring System integrates the MAX30102 optical sensor with the LPC2148 microcontroller to collect red and infrared sensor readings. The firmware processes these readings to estimate heart rate and SpO₂.

The system can display measurements on an LCD and transmit data to an IoT platform through an ESP-01 Wi-Fi module when those features are implemented.

## 📋 Project Details

| Category | Details |
|---|---|
| Project Title | Health Monitoring System Using MAX30102 |
| Project Type | Embedded Systems / IoT |
| Microcontroller | LPC2148 ARM7 |
| Programming Language | Embedded C |
| Sensor | MAX30102 |
| Communication Protocol | I²C |
| Wireless Module | ESP-01 Wi-Fi |
| IoT Platform | ThingSpeak |
| Development Environment | Keil µVision |
| Programming Tool | Flash Magic |

## 🎯 Objectives

- Measure heart rate using the MAX30102 sensor.
- Estimate blood oxygen saturation (SpO₂).
- Interface the MAX30102 with the LPC2148 using I²C.
- Process sensor readings using Embedded C.
- Display measurements on an LCD, if configured.
- Support remote monitoring through ESP-01 and ThingSpeak, if implemented.
- Demonstrate embedded firmware development and hardware–software interfacing.

## ⚙️ Key Features

- **Heart Rate Monitoring:** Uses optical sensor readings to estimate heart rate.
- **SpO₂ Estimation:** Processes red and infrared readings to estimate blood oxygen saturation.
- **I²C Communication:** Enables communication between the MAX30102 and LPC2148.
- **Embedded C Firmware:** Handles sensor configuration, data acquisition, and processing.
- **LCD Display:** Displays measurements and system status when configured.
- **IoT Integration:** Supports remote data visualization when wireless connectivity is implemented.

## 🧰 Hardware Components

| Component | Purpose |
|---|---|
| LPC2148 ARM7 Microcontroller | Main controller |
| MAX30102 Sensor | Heart rate and SpO₂ sensing |
| ESP-01 Wi-Fi Module | Wireless transmission, if implemented |
| 16×2 LCD | Displays measurements, if connected |
| Power Supply | Supplies power to the circuit |
| Connecting Wires | Hardware interconnections |

## 💻 Software and Technologies

- Embedded C
- ARM7 / LPC2148
- Keil µVision
- Flash Magic
- I²C Communication
- UART Communication
- Sensor Interfacing
- Firmware Development and Debugging
- ThingSpeak IoT Integration, if implemented

## 🔌 Peripheral Interfaces

### MAX30102 – I²C

The MAX30102 communicates with the LPC2148 through the I²C protocol.

- **7-bit I²C Address:** `0x57`
- **Interface:** I²C
- **Purpose:** Collects red and infrared optical sensor readings.

The firmware processes the collected readings to estimate heart rate and SpO₂.

### ESP-01 – UART and Wi-Fi

The ESP-01 can communicate with the LPC2148 through UART and transmit measurements over Wi-Fi to an IoT platform such as ThingSpeak.

### LCD Display

A 16×2 LCD can display heart rate, estimated SpO₂, and system status when the LCD interface is configured.

## 🏗️ System Architecture

The LPC2148 acts as the central controller and communicates with the MAX30102 sensor through I²C. Processed measurements can be displayed on an LCD or transmitted wirelessly through ESP-01 when implemented.

### System Block Diagram

![System Block Diagram](system_block_diagram.jpg)

*The LCD and IoT features are optional and depend on the implemented hardware and firmware.*

**System flow:**  
MAX30102 Sensor → I²C → LPC2148 ARM7 → LCD Display / ESP-01 → ThingSpeak

## 🔄 System Working

1. **System Initialization:** The LPC2148 initializes the required GPIO pins, I²C interface, and other configured peripherals.
2. **Sensor Initialization:** The firmware configures the MAX30102 sensor for red and infrared optical data collection.
3. **Data Acquisition:** The sensor collects optical readings, which are transferred to the microcontroller through I²C.
4. **Heart Rate and SpO₂ Estimation:** The firmware processes the collected sensor readings to estimate heart rate and blood oxygen saturation.
5. **Display of Measurements:** The measured or estimated values can be displayed on an LCD, depending on the implemented hardware.
6. **IoT Monitoring:** If the ESP-01 and ThingSpeak features are implemented, the measurements can be transmitted over Wi-Fi for remote visualization.

## 📷 Project Images

### Health Monitoring System Setup

The hardware setup of the Health Monitoring System using the LPC2148 ARM7 microcontroller and MAX30102 sensor.

![Health Monitoring System Setup](health_monitoring_setup_1.jpg)

### MAX30102 Sensor Setup

A view of the MAX30102 sensor and its hardware connections used for health monitoring.

![MAX30102 Sensor Setup](health_monitoring_setup_2.jpg)

## 📁 Project Structure

Health-Monitoring-System-Using-MAX30102/
├── MAX.c
├── Startup.d
├── Startup.lst
├── Startup.o
├── Startup.s
├── Timer1.c
├── all_defines.h
├── delay.c
├── delay.crf
├── delay.d
├── README.md
├── system_block_diagram.jpg
├── health_monitoring_setup_1.jpg
└── health_monitoring_setup_2.jpg


## 🧠 Concepts Demonstrated

- Embedded C programming
- ARM7 architecture
- LPC2148 microcontroller programming
- I²C communication
- MAX30102 sensor interfacing
- Heart rate and SpO₂ estimation
- UART communication
- Peripheral interfacing
- Firmware development and debugging
- Hardware–software integration
- IoT data transmission, if implemented

## 🚀 Future Enhancements

- Add real-time health data logging.
- Improve signal filtering and measurement processing.
- Add configurable alerts for selected thresholds.
- Build a web or mobile dashboard for remote monitoring.
- Store historical readings for later analysis.

## 👩‍💻 Author

Pulakanti Sai Niharika  
B.Tech – Electronics and Communication Engineering (ECE)  
GitHub: [P-SAI-NIHARIKA](https://github.com/P-SAI-NIHARIKA)

## 📌 Project Information

- Project: Health Monitoring System Using MAX30102
- Controller: LPC2148 ARM7
- Programming Language: Embedded C
- Sensor: MAX30102
- Domain: Embedded Systems / IoT

