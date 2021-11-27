# Requirements for Water level indicator
# Identifying Features
 - Easy installation.
 - Low maintenance.
 - Compact elegant design.
 - The Automatic water level controller ensures no overflows or dry running of pump    there by saves electricity and water.
 - Avoid seepage of roofs and walls due to overflowing tanks.
 - Fully automatic, saves man power.
 - Consume very little energy, ideal for continuous operation.
 - Automatic water level controller provides you the flexibility to decide for yourself the water levels for operations of pump set.
 - Shows clear indication of water levels in the overhead tank.

# State of art/Research
# Water level indicator with alarm system
![](https://s3.ap-south-1.amazonaws.com/rzp-prod-merchant-assets/payment-link/description/water-tank-500x500_DUGTX5ronA5YgC.jpg)

# SWOT ANALYSIS
# Strength
 - It is used to prvent water waste
 - Eliminating manual operations with a timer switch, the frustrations of manual monitoring water tanks are minimized.
 - Automatically adjusts water levels
 - Save money by using less electricity and water
 - Automatic operation saves you manual labor time
# Weakness
 - The rust, foul and deteriorate
 - Electronics are usually built separately
 - More difficult installation
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
Implementation of water level indicator
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
 - A constant 5v power supply is given to the microcontroller and rest of the circuit from a battery.
 - The tank has 9 conductive type sensors (other types of sensors have been mentioned earlier but in our project only conductive type are used) embedded into it and 8 wires of sensors out of 9 are connected to transistors and the 9th is connected to 5v+ supply.
 - The use of transistor is it acts as inverter (i.e. in on state gives low voltage at output and in non conducting state gives high voltage at its output), all transistors outputs are connected to PORTB of microcontroller.
Seven segment display is connected to PORTD. It is connected in common cathode fashion.
 - The Output for the 7th level is not only shown on seven segment display but also indicated with a discontinuous buzzer sound.
  - Output for the 8th level (i.e. tank full condition) is not only shown in seven segment display but also indicated with a continuous buzzer sound.

# Low level requirements
 - There is no water available in the source tank.
 - Intermediate level i.e. either of 3rd to 7th level.
 - There is ample amount of water available in the source tank.
