### What a Microcontroller Does

A microcontroller continuously:

1. Reads input signals (digital or analog)
2. Executes programmed logic
3. Updates outputs

This happens in a fast repeating loop. It converts code into electrical behavior.

### Sensor Communication Model

Sensors:
- Measure physical phenomena
- Store values in internal registers

Microcontroller:
- Initiates communication
- Requests data
- Interprets the returned bytes
- Decides what to do

## Abbreviations I didn&t know

IMU = motion sensor module
I2C = 2-wire communication protocol
SDA = data line
SCL = clock line
MEMS = microscopic mechanical structures inside sensors
ADC = converts analog voltage into digital number

## When Do We Use ADC?

Use ADC when:
- Reading raw analog voltage from a sensor

Do NOT use ADC when:
- Reading digital data via I2C, SPI, or UART
- The sensor already converts internally

## Digital Signals Are Voltage-Based

0 and 1 are represented by voltage levels.

In a 3.3V system:
- 0V ≈ LOW
- 3.3V ≈ HIGH

Incorrect voltage levels can:
- Cause communication errors
- Damage components

## Why I2C Uses Pull-Up Resistors

I2C lines use open-drain design:
- Devices can pull LOW
- Devices cannot drive HIGH

Pull-up resistors:
- Set the line HIGH by default
- Prevent bus contention
- Allow multiple devices to share the same wires safely

LOW always overrides HIGH.

## Digital HIGH and LOW

HIGH = wire at ~3.3V  
LOW = wire at ~0V (ground)

Pull-down:
Device connects wire to ground → voltage becomes 0V

Pull-up resistor:
Resistor connects wire to 3.3V → voltage becomes HIGH when no one pulls it down

## Multiple Devices Pulling LOW

If multiple devices pull the I2C line LOW:
- The voltage becomes 0V
- This is safe
- LOW always overrides HIGH

This works because devices do not actively drive HIGH.

## Current When I2C Line Is LOW

If:
- Vcc = 3.3V
- Pull-up resistor = 4.7kΩ
- Line is pulled to 0V

Then:

Current = 3.3 / 4700 ≈ 0.7mA

Voltage across resistor is still 3.3V.
Voltage is always a difference between two points.
