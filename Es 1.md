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
- Embedded systems might just run firmware - code written in Embedded C, C++, or MicroPython - iploaded via tools like Arduino IDE or PlatformIO.
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
## What is a Microcontroller
- Complete mini-computer on a single chip.
- CPU, memory, timers, and input.output pins, all built-in...
- Microcontrollers are purpose-built for real-time tasks.
- Energy-efficient, low-cost, and designed to do one job.
- Home devices, wearables, kitchen appliances, drones, and almost all IoT edge devices.
## Key Differennces
| Feature           | MPU                 | MCU                    |
| ----------------- | ------------------- | ---------------------- |
| Processing power  | High                | Moderate               |
| Memory            | External            | Built-in               |
| Power Consumption | High                | Low                    |
| Cost              | Expensive           | Budget-friendly        |
| Applications      | PC, Laptop, servers | Embedded / IoT devices |
## Real World Use Cases
- Smart camera
- Soil monitoring sensor
## Which one should you use
| Microprocessor                                                   | Microcontroller                         |
| ---------------------------------------------------------------- | --------------------------------------- |
| If your system :  Needs a full operating system like Linux      | If your system : Controls a single task |
| Handles complex tasks like voice recognition or video streaming. | Runs on battery or needs low power   |
## Role in Embedded  systems
In embedded systems, especially IoT, microcontrollers play a key role at the edge. They interact with sensors, collect data, and make instant decisions.
# Types of Embedded Systems
## What are Embedded Systems
An embedded system is a special-purpose computer built into a device to perform a dedicated function.
- Low power
- Real-time
- Small size
- High reliability
## Classification of Embedded Systems
Embedded systems are categorized based on functionality, performance, and architecture.
- Stand-alone
- Real-time
- Networked
- Mobile
- Small/Medium/Large scale
- Hybrid
## 1. Stand-Alone Embedded Systems
These systems work independently. They get inputs, proocess them, and give outputt.
### Examples:
- Washing machine
- Microwave oven
- MP3 player
## 2. Real-Time Embedded Systems
Real-time systems must react within a specific time limit. These are mission-critical.
- Hard real-time: Failure to respond in time results in a disaster (e.g., pacemaker, anti-lock brakes)
- Soft real-time: Occasional delays are tolerable (e.g., video streaming)
## 3. Networked Embedded Systems
These are connected to a network or internet, enabling communication with other devices.
### Examples:
- Smart home automation systems
- IoT-enabled irrigation systems
- Industrial IoT sensors
## 4. Mobile Embedded Systems
Mobile embedded systems are portable and often battery-powered.
### Example:
- Smartwatches
- Digital cameras
- Fitness bands
## 5. Small, Medium & Large-Scale Systems
This classification is based on complexity, memory, and performance.
### Small-scale:
- 8/16-bit microcontrollers (e.g., calculators, remote controls)
### Medium-scale:
- More complex, 16/32-bit controllers (e.g., printers, vending machines)
### Large-scale:
- High performance, often running RTOS (e.g., avionics systems, industrial automation)
## 6. Hybrid Embedded Systems
Many modern systems are hybrid, combining types.
#### A smart car is stand-alone, networked, real-time, and mobile.
### Examples:
- Autonomous vehicles
- Smart healthcare devices
- Drones
###
| Stand-alone | Self-contained devices     |
| real-time   | Time-sensitive tasks       |
| Networked   | Connected to other systems |
| Mobile      | Portable and efficient     |
| Scale-based | Resource complexity        |
| Hybrid      | Combines multiple types    |
