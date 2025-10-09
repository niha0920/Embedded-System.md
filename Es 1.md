# Introduction to Embedded Systems
## Definition 
Dedicated computer designed to perform one or a few specific tasks - reliably and efficiently.
- It's usually tiny, highly optimized, and hidden inside another device.
- Always working behind the scenes.
## Characteristics of Embedded Systems 
key characteristics
- Dedicated function
- Work in real time
- Limited resources
- Low power consumption
## Embedded Systems vs General Computers
- PC is designed to run many applicatons - games, browsers, video editing.
- An embedded system is built to do just one job - but do it very efficiently.
## Real-World examples of Embedded Systems
Here are some real world examples
- Fitness band
- Washing machine
- Fuel, airbags, braking systems in cars
- Infusion pumps, heart monitors, ventilators in hospitals
## Embedded System in IoT
IoT is all about connecting devices to the internet - and embedded systems make it possible.
### A small irrigation system in agriculture uses:
- Sensors to check soil moisture
- A microcontroller to process data
- Wi-Fi to send info to the cloud
- And actuators to control water flow
# Embedded Systems vs General Systems
## General Purpose Systems
These are machines designed to perform a wide variety of tasks. Examples include laptops, desktops, smartphones, tablets.
- They have powerful processors, run complex operating systems like Windows, Linux, Android, and can support tons of apps simultaneously - games, browsers, video editors, IDEs.
## Embedded System 
It's a small computer - usually a microcontroller or microprocessor-based device - that performs a specific tassk.
- Controlling temperature
- Managing fuel injection
- Monitoring heartbeat
- Measuring soil moisture
## Key Differences
| Feature           | General Purpose System            | Embedded System                       |
| ----------------- | --------------------------------- | ------------------------------------- |
| Purpose           | Multiple tasks                    | One specific function                 |
| OS                | Full OS (WINDOWS, LINUX, ANDROID) | Minimal or RTOS or bare metal         |
| Hardware          | Powerful CPU, GPU, HDD, RAM       | Simple MCU, Flash, EEPROM             |
| User Interface    | Keyboard, Mouse, Screen           | Often no interface (or buttons, LEDs) |
| Connectivity      | Wi-Fi, Bluetooth, LAN, USB, etc.  | May have limited or specific I/O      |
| Power Consumption | High                              | Very Low                              |
| Cost              | Higher                            | Lower (can be <$2 MCU)                |
| Examples          | Laptop, Phone, PC                 | Smartwatch, Washing Machine, Drone    |
## Performance and Interaction
- General-purpose systems are made for constant human interaction. You type, click, speak, swipe.
- Embedded systems often work in the background, interacting with sensors, motors, or machines.
## Software Environment Comparision
- A general-purpose system supports compilers, browsers, apps, games.
- Embedded systems might just run firmware - code written in Embedded C, C++, or MicroPythin - iploaded via tools like Arduino IDE or PlatformIO.
- Some run on RTOS like FreeRTOS, Zephyr, or even TinyOS for real-time control.
## Real World Applications
- Smartphones
- Fitness band
- Laptop
- Automatic door
- Drone
## Where they work together
A  smart farming system may use:
- Embedded nodes (with ESP32) in the field
- Cloud server on a general-purpose system
- Smartphone app to control and view data
#### So, both systems complement each other in smart solutions.
# Microprocessors vs Microcontrollers
## What is a Microprocessor?
- Central processing unit on a single chip.
- Handles computations, decision-making, and executes instructions.
- Needs help from external memory, I/O devices, and other components to function as a system.
- Laptop, desktop PC, and even powerful AI gateaways.
#### Designed for general-purpose tasks - browsing, multitasking, gaming, or managing heavy data operations.
