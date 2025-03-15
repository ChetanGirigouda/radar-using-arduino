# Radar system using Arduino

## Overview
This project is an **Ultrasonic Radar System** that uses an **Arduino Uno**, an **HC-SR04 Ultrasonic Sensor**, and a **Tower Pro 9G Micro Servo Motor** to detect objects in its vicinity. The system visualizes the detected objects on a **radar-like display** using the **Processing IDE**.

## Components Used

| **Component**                                       | **Pin Name**         | **Connected To (Arduino)**|
|-----------------------------------------------------|----------------------|---------------------------|
| **Arduino Uno R3 SMD Compatible Development Board** | -                    | -                         |
| **Ultrasonic Sensor (HC-SR04)**                     | VCC                  | 5V                        |
|                                                     | GND                  | GND                       |
|                                                     | Trig                 | Digital Pin 10            |
|                                                     | Echo                 | Digital Pin 11            |
| **Servo Motor (Tower Pro 9G)**                      | VCC (Red)            | 5V                        |
|                                                     | GND (Brown/Black)    | GND                       |
|                                                     | Signal (Orange/Yellow) | Digital Pin 12          |

## How It Works
- The **servo motor** rotates from **15° to 165°** and back.
- The **HC-SR04 ultrasonic sensor** measures the distance to objects in its path.
- Data (angle and distance) is sent to the **Processing IDE** via **serial communication**.
- The **Processing script** visualizes the scanned objects on a radar-like interface.

## Installation & Usage
### **1. Setup Arduino Code**
- Install the **Arduino IDE** if not already installed.
- Connect the Arduino Uno to your PC.
- Upload the `arduino_radar.ino` script to the board.

### **2. Setup Processing Code**
- Install the **Processing IDE**.
- Install the `processing.serial` library (if not already installed).
- Run the `processing_radar.pde` script.

### **3. Hardware Setup**
- Connect the components as per the wiring table above.
- Power up the Arduino and open the **Processing IDE** to visualize the radar.

## Files in This Repository
- `arduino_radar.ino` - Arduino sketch to control the servo and sensor.
- `processing_radar.pde` - Processing script for visualizing the radar system.
- `README.md` - This documentation file.

## Demo
![radar using arduino](https://github.com/user-attachments/assets/50248fdb-19fc-47bd-9a47-898394bba4b6)


## License
This project is open-source and free to use for educational and research purposes.

## Contributing
Feel free to contribute by submitting a **pull request** or **raising an issue** for improvements or bug fixes.

---


