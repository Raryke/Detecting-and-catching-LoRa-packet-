LoRa DETECTING, CATCHING and ANAALYSIS
This project focuses on capturing and analyzing LoRa communication packets between Arduino sensors and a Dragino Gateway using RTL-SDR and various software tools. 
The system allows monitoring of temperature, humidity, and smoke detection data transmitted over LoRaWAN networks.
This documents provides brief instructual manual, for more detailed procedure see the report 

PROJECT OVERVIEW:
The project implements a complete IoT sensor monitoring system with:
- Arduino board with temperature, humidity and smoke sensors
- Dragino LG01-N LoRaWAN gateway
- RTL-SDR receiver for packet capture
- The Things Network (TTN) integration
- Packet analysis and decryption capabilities

PREREQUISITIES
The following hardware is required:
- Arduino Uno with LoRa Shield
- Temperature, humidity and smoke sensors
- Dragino LG01-N Gateway
- RTL-SDR dongle (R820T/RTL2832U)
- Computer running Linux (Ubuntu 22.04 recommended)

SOFTWARE REQUIREMENTS:
- Docker
- GNU Radio (installed via Docker)
- RTL-SDR drivers and tools
- Arduino IDE
- The Things Network account

INSTALLATION AND SETUP:
- Install Docker and configure it to run without sudo:
- Install GNU Radio with LoRa support using Docker:

CONFIGURE THE DRAGINO GATEWAY:
- Connect to gateway web interface
- Configure network settings
- Register gateway on TTN
- Set frequency to 868.1 MHz


SET UP ARDUINO:
- Install required libraries (LMIC, LoRa-raw, DHTlib)
- Configure device credentials from TTN
- Upload provided sensor code
  
USAGE:
- Start the Docker container with GNU Radio:
- Launch GNU Radio Companion and open the provided capture flow graph
- Connect RTL-SDR and start packet capture
- Analyze captured packets using the included JavaScript decryption tool:
-View decoded sensor data in TTN console using CayenneLPP format

DOCUMENTATION
- Complete hardware setup
- Software installation guides
- Network configuration
- Packet structure analysis
- Decryption process
- Troubleshooting tips

CONTRIBUTING
This project was developed as part of a student technical project at Slovak University of Technology in Bratislava. 
AUTHORS
Miroslav Čech, Branislav Dorčák, Nikolas Merva, Lukáš Rarogiewicz 
