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
- The protocol is managed by software stack. This increases processing overheads on the µP and µC.
# Opportunities
 - Can be used in water tanks to control water levels
 - Automatically turn ON/OFF pumps
 - Can be used in factories, commercial complexes, apartments, home.
#  Threats
 - Most float switches are outdated
 - No LED indicator lights
# 4W's and 1H

# Who
B.Meghana try to implement a problem statement
# What
Implementation I2C LCD With clock
# Where
 - Cooling tower water level control
 - Sewage pump level control
 - Water level control
 - Pump controller
 - Stream level monitoring
 - Irrigation control
 - Police vans in emergency
 # How
 - This application is implemented using C programing language
# High level requirements
 - Sends an alert to let you know water is too high or too low
 - Automatically adjusts water levels
 - Save money by using less electricity and water
 - Can help avoid seepage of roofs and walls due to tanks overflowing
 - Automatic operation saves you manual labor time
 - Consumes a small amount little energy, perfect for on-going operations
 - Indicates water levels in any type of storage tank or body of liquid
 - A water alarm is loud so you can easily hear it
# Low level requirements
 - There is no water available in the source tank.
 - Intermediate level i.e. either of 3rd to 7th level.
 - There is ample amount of water available in the source tank.
