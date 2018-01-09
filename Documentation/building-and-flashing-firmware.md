# Prerequisites
Before we can build the firmware, we need to download and install XC16 and MPLAB-X, the toolchain and IDE used to compile firmware for the Bus Pirate's PIC24 microcontroller. 

## XC16
XC16 is available from Microchip's website at http://www.microchip.com/mplab/compilers

Scroll down, Click on the Downloads tab, and download XC16 (not XC8 or XC32) for your platform.

On Linux, you may have to make the file executable and run it from the command line
```
chmod +x xc16-*.run
./xc16-*.run
```
Follow the prompts and select the option to Add XC16 to the PATH environment variable.

## MPLAB-X
MPLAB-X is available from Microchip's website at http://www.microchip.com/mplab/mplab-x-ide

Scroll down, Click on the Downloads tab, and download MPLAB-X for your platform.

On Linux, you have to un-tar the installation script and make it executable before you can run it
```
tar xf MPLABX-*.tar
chmod +x MPLABX-*.sh 
./MPLABX-*.sh
```
Follow the prompts to install MPLAB-X

# Building
Open MPLAB-X

Click File>Open Project and navigate to Bus_Pirate/Firmware/busPirate.X

Select BusPirate_v3 or BusPirate_v4 from the dropdown menu in the toolbar

Click the hammer in the toolbar.

Your firmware will be saved in Bus_Pirate/Firmware/busPirate.X/dist/BusPirate_v*/production/busPirate.X.production.hex

# Flashing
