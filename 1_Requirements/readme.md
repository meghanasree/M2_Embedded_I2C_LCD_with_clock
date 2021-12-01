# Requirements for Water level indicator
# Identifying Features
- Communicate on a 2-wire I2C bus
-  API compatible with the current character LCD component
- One component may drive one or more LCDs on the same I2C bus
- Can coexist on an existing I2C bus if the PSoC is the I2C master
- Support for the NXP PCF2119x command format

# State of art/Research
# Water level indicator with alarm system
![](https://s3.ap-south-1.amazonaws.com/rzp-prod-merchant-assets/payment-link/description/water-tank-500x500_DUGTX5ronA5YgC.jpg)

# SWOT ANALYSIS
# Strength
- I2C requires only two wires for communication unlike SPI which requires four. Hence it minimizes interconnections between ICs due to 
   fewer pins and also fewer PCB tracks. This results into smaller and less expensive PCBs.
- The addressing is very simple and does not need any CS lines to add extra devices like SPI. 
- Hence addition of any extra device is very easy.
- It uses open collector bus design and hence there is flexibility to use voltage on the bus.
-  Moreover slew rates are limited.
- It uses flow control.
- It is easy to perform diagnosis and debugging. Hence it is easy to trace malfunctionalities.
- ICs can be added or removed from the hardware without affecting any other circuits on bus.
# Weakness
-  The hardware complexity increases when number of master/slave devices are more in the circuit.
- It is half duplex mode of communication.

# Opportunities
 - Can be used in water tanks to control water levels
 - Automatically turn ON/OFF pumps
 - Can be used in factories, commercial complexes, apartments, home.
#  Threats
 - The protocol is managed by software stack.
 -  This increases processing overheads on the µP and µC.
# 4W's and 1H

# Who
B.Meghana try to implement a problem statement
# What
Implementation I2C LCD With clock
# Where
 - This clock only counts for 1 hour and then starts over again. Minor changes are needed to write a 24 hour clock, 
  but for now I thought this is a good start. My clock is not so accurate at the moment. It’s about 2 seconds a minute to fast.
  To get the clock more accurate you can change the CMR_SECOND and the CMR_MINUT number in the timer4clocklib.h.
 # How
 - This application is implemented using C programing language
# High level requirements
 - Put the correct voltages on all the lcd pins for the first 4 bits of a byte you want to send.
 - Set the enable pin high for more then 450 nano seconds and keep the rest of the pins the same.
 - Set the enable pin low for more then 37 micro seconds and keep the rest of the pins the same.
 - Do the last 3 steps again, but now for the last 4 bits of 8.
# Low level requirements
 - Again I used the same framework to get the lcd working simultanesly 
  with other devices in the future and for now I only added 1 led to test the multi threating.
