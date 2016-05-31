# LattePanda FRC Driver Station
This is Garnet Squadron's next iteration to the control board. This one dumps the typical laptop and opts for a LattePanda Windows 10 single-board computer with Arduino Leonardo Co-Processor. This repo will hold Windows software, Arduino firmware, design files, and documentation.

## Features
- 16 20mA LED Outputs
- 16 General Purpose I/O
- 16 Analog Inputs
- 16 PWM Outputs
- Backup battery for safe shutdowns
- Auto power-on with AC connect
- LattePanda 
	- Windows 10 Professional
	- 4GB RAM
	- 64GB SSD
	- Intel Cherry Trail Z8300 Quad Core 1.8GHz
	- 3 USB Ports (2 USB 2.0, 1 USB 3.0)
	- Ethernet 10/100
	- 7" Capacitive Touch Screen (1024 x 600)
	- WiFi
	- Bluetooth

## How it works
The Arduino Leondaro connects with I/O expansion chips:

- Microchip MCP23017 - 16-Bit GPIO Expander with I2C Interface
- NXP PCA9685 - 16 channel PWM Driver
- TI CD74HC4067 Analog Multiplexer
- TI TLC59282 16-Channel Constant-Current LED Driver

There is a 2000 mAh LiPo battery that can provide backup power for an estimated 1 hour. While the battery life isn't great, the intended purpose is to provide power long enough to shutdown Windows 10 between matches. Override inputs will be available to:

- Keep the board powered on until battery life reaches ~5%
- Power button to turn on the system even when off of AC power.




 

