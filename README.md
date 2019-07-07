# CH2i Arduino Custom Boards Definition

An Arduino core for some of my custom boards such has [Mini-Lora](https://github.com/hallard/Mini-LoRa) that have been optimized with optiboot bootloader and different serial speed to increase and improve uploading.
This requires at least Arduino IDE v1.6.2, where v1.8.6+ is recommended. 


## Bootloader 
Your board should have the bootloader already flashed, it's not the scope of this repo. Everything to burn bootloader is explained [here](https://github.com/hallard/Pro-Mini-ICSP-FTDI)

## How to install

Click on the "Download ZIP" button in the upper right corner. Exctract the ZIP file, and move the extracted folder to the location "**~/Documents/Arduino/hardware**". Create the "hardware" folder if it doesn't exist.

After extraction, you should have something like "**~/Documents/Arduino/hardware/ch2i-arduino-boards-master**", of course you can rename folder to "**~/Documents/Arduino/hardware/ch2i**"
Open Arduino IDE, and a new category in the boards menu called "CH2i Boards" will show up.

## Getting started with MiniCore

Ok, so you're downloaded and installed, ready to upload but how to get started? Here's a quick guide:

* Open the **Tools > Board** menu item, and select a CH2i Boards compatible microcontroller, example `Mini Lora`
* Select your prefered clock frequency. **16 MHz** is standard on most Arduino boards but 3.3V Boards shoudl be 8MHz.
* Select uploading serial speed depending on which bootloader speed you flashed into your Arduino board.

For example, if you flashed bootloader `optiboot_flash_atmega328p_250000_8MHZ.hex`

 * select 250KBps for serial speed
 * slect 8MHz for Clock



