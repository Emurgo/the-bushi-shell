## CAD Comparison Analysis:

[CADComparison.md](docs/CADComparison.md)

## Pi Research:
[PiResearch.md](docs/PiResearch.md)

* List of different 3D printing plastics and their properties: 

   [3DPrinterPlastics.md](docs/3DPrinterPlastics.md)
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

[RockPiDimensions.md](docs/RockPiDimensions.md)    

# Prototype 1 
## Codename: Hideyoshi 

- This case would be different than the current ones out in the market. With a sleak curved design, this case would not only be able to protect the case, but look aestheically pleasing as well to distinguish our design from the rest of the community. In turn, more people would be incline to modify the design to fit their needs. 

#### Lid design: 
     - After conducting research on the different designs of casings for microcomputers, stakeboxes, and other microprocessing devices, I came to the conclustion that this system should have a double locking system to ensure that the case stays in place even in the event of a fall. 
     - The case accomplishes this by having 3 step locking system bound to a curve. These are the steps to open the case: 
         
           1.) Pull the lid slightly
           2.) Slide the lid down the curve of the case until it stops
           3.) Pull off the lid for access to the internal devices
      
    - By implementing this system, it would be able to prevent premature removal of the top protection of the device.

      Note: There are still some modificaitons to be done. 

      - Currently, this system is still undergoing statical analysis to see if it is ready for production. 

### ** **Discontinued for risk of printing difficulty** **

# Prototype 2 
## Codename: Oda

Please read: 
[Pre-design](docs/Pre-design.md)

### Plan:
 - Case will be made up of a top and a bottom components.

 - **Case Dimensions (Estimate):** 95 x 60 x 30 (mm) 
 - There will be three different lock systems (clip, double slot, and pin lock) to ensure that the case does not come off unless the user requests it. 

 #### Bottom 

    - A Heat sink will be included alongside with the Pi  that would require a 1-3mm washer 
  
    - Ensure a 0.05mm threshold between the case and the associated port. This is to make sure that the case will truely fit the Pi. 
   
    - Creation of male connection pins on the area where holes appear on the Pi. The pins are design to be one element that would aid on the prevention of movement of the device.
   
    - Design bumps that will properly connect to a double lock device on the top case.

   ##### Possible Add-on Ideas:
     - Corner clips to keep the pi in place while not causing damage to the corners.
     - An upper enclosure that would hug around the pi when the case is closing.

 #### Top

##### Locking Mechanisms
    - The Lid of the case will consist of 3 different locking mechanisms:
    
    1.) Clip locks: This clip would attach when the system is fully in position to prevent movement of the case as a whole.

    2.) Screw lock: For the Pi and heatsink screws will be included on all four corners to secure the Pi and heatsink in place. 

    3.) Double-Slot: A zig-zag lock that would require the user to slightly pull up, slide forward, then take out the lid. This is to ensure that the lid does not come off unless the user desires. 




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