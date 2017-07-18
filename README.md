# PI2GENESIS-USB-HUB
PCB for placing a RaspberryPi3 into Nerd Block's Genesis USB Hub and getting 15KHz RGB Video out of it.


PCB SPECS:
----------------
10.0 x 5.0 cm
1.2 mm Thickness
HASL


Connects to a Raspberry PI 3(b) inside the housing of Arcadeblock(Nerdblock) Genesis USB Hub and turns it into a mini-videogame-system.
Video-Output is 15KHz-RGB. Needs configuration settings to output correct video. (Like Pi2Scart or Pi2Jamma)
Uses the original USB-sockets from the USB-Hub's PCB.

Additional Modding:
-DC-Power-Input (5V)
-Video-Out via 8-Pin-MiniDIN Socket
-optional separate H- and V-Sync via dedicated cinch-sockets and cinch-to-bnc cables for studio monitors/PVM

Installation Notes:
-desolder original USB-sockets and install them on the pcb
-solder PCB to GPIO-pins
-connect usb-pins with cables (D+ and D- Lines 1-4)
-connect usb-power-pin to one of the usb-sockets on the PI
-connect AUDIO from PI to SND-L and SND-R pins
-connect VIDEO-OUT to AV-Socket
-connect POWER and GND from PSU to 5V-IN
-connect POWER and GND from 5V-OUT to PI-Power-Input (miniUSB-port)
-when AUDIO has noise, use a groundloop-isolator between the connetction
