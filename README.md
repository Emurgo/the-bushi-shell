## CAD Comparison Analysis:

[CAD Programs](docs/CADComparison.md)

## Pi Research:
[Pi Research Findings](docs/PiResearch.md)

* List of different 3D printing plastics and their properties: 

   [3D Printer Plastics](docs/3DPrinterPlastics.md)
# Case Design
### Objective:
      - Provide a complete open source guide to run a Cardano Rust full node in single-board computers like Rockpi
      - Open source 3D printable case designs
     

### Requirements:
     - The casing must withstand an average impact force of at least 16 N to withstand a fall from a table. 
     - Must have room for two LEDs for displaying the power and the status
     - Ensure that all essential ports are exposed with at least 0.4mm of tolerence for easier installation. 
     - Find a material that can economically absorb impact force to ensure the case can protect the Pi in different environments. 
     - Ensure that the casing can be aesthetically pleasing to attract more people to download and improve the case. 

### Microcomputer Dimensions:

[RockPi](docs/RockPiDimensions.md)    

# Prototype 1 
## Codename: [Hideyoshi](docs/Hideyoshi.md)
### ** **Discontinued for risk of printing difficulty** **

# Prototype 2 
## Codename: [Oda](docs/Oda.md)
### ** **Discontinued for severe design issues** **

# RockPi Configuration

## Hardware needed
 - RockPi 4B (With Dualband 2,4/5GHz WLAN/Bluetooth 5.0)
 - A 32GB or 64GB eMMC 
 - HDMI Cable
 - USB-C Power cord
 - eMMC to microSD adapter
 - USB card reader or microUSB to USB card reader
 - USB Keyboard and Mouse
 

## How to install the Armbian OS to an eMMC

 ### 1.) Download 
 - Download the <a href = 'https://www.armbian.com/rock-pi-4/'>Armbian</a> Buster OS 

 - Install <a href = 'https://www.balena.io/etcher/'> Etcher</a> for writing the OS to your storage device.

 ### 2.) Write
 - After the OS and the writing tool are both installed, plug in the eMMC and format it using an <a href ='https://www.sdcard.org/downloads/formatter/' > SD card formatter</a>.

- Unzip the OS using <a href = 'https://www.7-zip.org/'>7-zip</a> (Windows), <a href = 'https://www.keka.io/en/'>keka</a> (Mac OS), or 7z (Linux) and use Etcher to write the unzipped image file to the eMMC. 

 ### 3.) Boot
- 