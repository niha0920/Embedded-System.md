# Basic Electronic Components
## Resistors
A resistor resists the flow of electric current. It helps control voltage and current in a circuit.
### Ohm's Law:
V = I * R
#### Voltage = Current * Resistance
Measured in Ohms (Ω).
### Applications:
- Limiting current to an LED.
- Voltage dividers.
- Pull-Up and pull-down resistors in microcontrollers.
## Example: An LED Protected by a Resistor
- Without a resistor, components like LEDs would burn out instantly when connected to a power supply.
- That's why proper resistance calculation is critical.
### Use the color code to quickly determine resistor values!
## Capacitors
A capacitor stores electrical energy temporarily and releases it when needed.
#### Units: Farads (F)
### Basic Formula:
Q = C * V
#### Charge = Capacitance * Voltage
### Applications:
- Power supply filtering (smoothing ripple).
- Energy storage.
- Timing circuits (RC circuits).
## Diodes
- Allow current in one direction only.
- Block current in the opposite direction.
- Symbol: Arrow with a bar (|>) in circuit diagrams.
### Types of Diodes:
- Standard Diode: Protection against reverse polarity.
- Zener Diode: Voltage regulation.
- Light Emitting Diade (LED): Emits light.
## Transistors
### Types:
- BJT (Bipolar Junction Transistor) - current-controlled.
- MOSFET (Metal-Oxide-Semiconductor FET) - voltage-controlled.
### Three parts:
- Base (B)
- Collector (C)
- Emitter (E) - for BJT
#### (For MOSFETs: Gate, Drain, Source.)
### Main Functions:
- Switch: Turn circuits on / off electronically.
- Amplifier: Boost weak signals (used in radios, audio devices).
## Example
Lighting an LED through a resistor, controlled by a transistor acting as a swicth!

# Power Supply Design and Basics of PCB
## What is a Power Supply?
A power supply is an electrical device that provides the necessary voltage and current to your circuit.
- Convert: AC to DC (or change voltage levels)
- Regulate: Provide a stable output, even if input varies
- Filter: Remove noise and ripple
- Protect: Prevent overload, short circuit, etc.
## Types of Power Supply
Power supplies come in various flovors. Let's explore the main categories:
1. Linear Power Supplies
2. Switch Made Power Supplies (SMPS)
3. Battery Power Supplies
4. USB Power
## Linear Power Supplies
Use a transformer, rectifier, and  linear regulator like the famous 7805
- Simple and low noise
- But less efficient - because excess voltage is wasted as heat
## Switch Mode Power Supplies (SMPS)
- Use high-frequency switching to step down or up voltages.
- Examples: Buck, Boost, Buck-Boost converters
- Much more efficient
## Battery Power Supplies
- Use rechargeable or primary batteries.
- Often include battery management systems (BMS) for charging, protection, and voltage regulation.
## USB Power
- Widely used in IoT devices.
- Typically delivers 5V with current limits (500mA-3A depending on USB type)
## Components of Power Supply Design
1. Transformer (in AC-DC supplies)
2. Bridge Rectifier
3. Filter Capacitor
4. Voltage Regulator
5. Inductor (in SMPS)
6. Zener Diodes
7. Protection Devices
## Design Considerations
- Input and Output Voltage
- Load Current Range
- Efficiency Requirements
- Thermal Dissipation
- Size Constraints
- Cost and Availability
## Basics of PCB Design
A PCB is where your power supply and components physically sit. It connects them using copper traces instead of wires.
### Key layers:
#### Copper Layer:
For signal / power routing
#### Silkscreen:
Labels and component names
#### Soldermask:
The green coating that prevents shorts
## PCD Design Tools
KiCad, Eagle, EasyEDA, Altium Designer
## Basic Steps
- Schematic Design - Place and connect components logically.
- Component Placement - Arrange components physically on the board.
- Routing Traces - Connect the pins with appropriate width.
- DRC Check - Verify design rules before generating Gerber files.
- Export Gerber Files - used for manufacturing.
## Power Supply Layout in PCB
Power circuits need careful PCB layout to avoid heat, noise, and voltage drop.
### PCB Design Tips for Power Supplies:
- Thick Power Traces
- Short and Direct Paths
- Ground Planes
- Thermal Reliiefs
- Bypass capacitors
- Keep Feedback Traces Short
#### Good Layout = stable voltage and long component life.

# Introduction to Sensors and Actuators
## What are Sensors and Actuators?
- Sensors are devices that detect physical phenomena.
- Actuators receive control signals and convert them into physical action
### Examples:
- Temperature Sensor (e.g., LM35)
- Motion Sensor (e.g., PIR)
- Servo Motor as an actuator
- Relay module
## Classification of Sensors
### Based on the type of input:
- Thermal
- Mechanical
- Optical
- Chemical
### Based on signal output:
- Analog sensors
- Digital sensors
### Active vs. Passive Sensors
- Active: Require external power
- Passive: Do not require power
## Classification of Actuators
Actuators can be classified as:
- Electrical Actuators (e.g., Motors, Solenoids)
- Hydraulic Actuators (fluid-powered)
- Pneumatic Actuators (air-powered)
- Thermal or Magnetic Actuators (e.g., Bimetallic strips, Relays)
## Working with Embedded Systems
In embedded systems, sensors and actuators interface with microcontrollers:
- Sensors send data to the microcontroller via ADCs (for analog) or directly via GPIOs (for digital).
- Actuators are driven by the controller via drivers or transistors (because microcontrollers can't supply high current directly).
## Communication Protocols and Sensor Interfacing
Advanced sensors use protocols for more accurate and complex data transmission:
- I@C - e.g., MPU6050 accelerometer
- SPI - e.g., sensors in SD cards, displays
- UART - GPS modules, Bluetooth
- 1-Wire - e.g., DS18B20 temperature sensor
## Smart Sensors and IoT Integeration
Smart Sensors come with built-in signal processing, calibration, and communication interfaces.
### Examples in IoT:
- DHT11 sensor with Wi-Fi (ESP8266)
- Air quality sensors (MQ135) sending data to cloud dashboards
- Actuators controlled via apps (e.g., home automation systems)
## Real-World Applications
Real-world applications include:
- Smart Agriculture - soil moisture sensors and irrigation control
- Smart Homes - motion sensors, light actuators
- Healthcare - biosensors and infusion pumps
- Industrial Automation - pressure sensors and robotic arms

# Analog and Digital Signals in Embedded Systems 
## What is a Signal?
A signal is a way of carrying information. In electronics, it usually means a change in voltage or current over time.
### Signals come in two types:
- Analog - smooth, continuous signals.
- Digital - step-by-step, binary sugnals.
## Analog Signals - Continuous Worls
Analog signals are continuous. That means the voltage or current can take any value within a range.
- Temperature sensors like thermistors.
- Sound waves picked up by microphones.
- Light intensity measured by LDRs.
## Digital Signals - The Language of Computers
Digital signals are discrete. They only have two levels: HIGH and LOW.
- In most systems, HIGH is 5 volts, and LOW is 0 volts.
- Digital signals are ideal for processing by microcontrollers.
## Analog vs Digital
| Feature          | Analog          | Digital                  |
| ---------------- | --------------- | ------------------------ |
| Nature           | Continuous      | Discrete                 |
| Accuracy         | High            | Depends on resolution    |
| Noise resistance | Low             | High                     |
| Processing       | Needs ADC       | Direct Logic             |
| Examples         | Microphone, LDR | Button, Proximity Sensor |
## How Microcontrollers Handle Signals
In embedded systems, microcontrollers like Arduino, STM32, and ESP32 can handle both types of signals.
- ADC - Analog-to-Digital Converter.
- PWM or DAC - Digital-to-Analog Converter.
## Deeper into ADC and DAC
- ADC converts an analog signal to a digital value - often a 10-bit or 12-bit number. That means you get 1024 or 4096 steps of resolution.
- DAC does the reverse - converting a digital number to a voltage, to control things like speakers or motors.
## Real World Applications
- In smartphones - microphones use analog input, touch sensors use digital.
- In smart agriculture - analog soil moisture sensors, digital rain sensors.
- In healthcare - analog ECG sensors, digital heart rate monitors.
- In home automation - analog light detection, digital motion detection.
## Mixed Signal Systems
- Most embedded systems today are mixed-signal systems - meaning they handle both analog and digital signals.
- Microcontrollers need to read analog data, process it digitally, and sometimes output analog responses.
## Analog and Digital in Modern IoT
- In IoT systems, the analog-digital combination is everywhere.
- Environmental data like temperature, humidity, sound - all start as analog.
- They're converted , processed, and shared digitally over Wi-Fi or BLE.
- Understanding how analog and digital signals work is key to building robust IoT systems.

# Signal Conditioning in Embedded Systems (The Bridge Between Sensors and Microcontrollers)
## What is Signal Conditioning?
- Signal conditioning refers to manipulating an analog signal to make it suitable for digitization or further processing.
- It prepares real-world signals which are often noisy, weak, or in incompatible formats so that microcontrollers and ADCs can interpret them correctly.
## Why do we Need Signal Conditioning?
- Amplification
- Filtering
- Level Shifting
- Clipping
## Common Signal Conditioning Techniques
Most commonly used signal conditioning techniques in embedded systems:
- Amplification
- Filtering
- Isolation
- Level Shifting & Clipping
- Linearization
## Practical Example: Temperature Sensor
You have an LM35 sensor that outputs 10 mV/C. You want to measure temperature with higher resolution and filter out 50 Hz noise.
## Signal Conditioning ICS & Modules
### INA333 or AD620
- Instrumentation amplifiers
### MAX4051
- Analog multiplexer
### ISO124
- Isolation amplifier
### LT1167
- Low-noise precision amplifier
## Embedded Systems and ADC Interface
Here's what you should remember when interfacing a conditioned signal with an ADC:
- The signal should be within the ADC voltage range.
- Avoid floating inputs - use pull-down resistors if needed.
- Choose the right ADC resolution based on your application.
## Real-World Applications
- Weather stations - measuring temperature and humidity
- ECG machines - capturing electrical heart activity
- Automotive systems - it helps read signals from wheel speed sensors, accelerometers, and pressure sensors.
