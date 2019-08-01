## Hardware needed
 - RockPi 4B (With Dualband 2,4/5GHz WLAN/Bluetooth 5.0)
 - A 32GB or 64GB eMMC 
 - HDMI Cable
 - USB-C Power cord
 - eMMC to microSD adapter
 - SD card reader or microSD to SD card adapter
 - USB Keyboard and Mouse
 

## How to install the Armbian OS to an eMMC or microSD 

 ### 1.) Download 
 - Download the <a href = 'https://www.armbian.com/rock-pi-4/'>Armbian</a> Buster OS 

 - Install <a href = 'https://www.balena.io/etcher/'> Etcher</a> for writing the OS to your storage device.

 ### 2.) Write
 - After the OS and the writing tool are both installed, plug in the eMMC or MicroSD and format it using an <a href ='https://www.sdcard.org/downloads/formatter/' > SD card formatter</a>.

- Unzip the OS using <a href = 'https://www.7-zip.org/'>7-zip</a> (Windows), <a href = 'https://www.keka.io/en/'>keka</a> (Mac OS), or 7z (Linux) and use Etcher to write the unzipped image file to the eMMC or MicroSD. 

 ### 3.) Boot
- Install the memory storage system into the microcomputer and turn on the system. 

- When first loging in type:
   - Username: root
   - Password: 1234
   
   After logging in for the first time, the system will ask you to come up with username and password that would be used for future logging in. However, the administrative account will still be root but the system will require you to make a new password for that one too. 

- One logged in the Armbian OS should be sucessfully installed and ready to run the program we will use for this staking device called [Jormungandr](jormungandr.md)