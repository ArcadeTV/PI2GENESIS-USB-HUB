# PI2GENESIS-USB-HUB

PCB for placing a RaspberryPi3 into Nerd Block's Genesis USB Hub and getting 15KHz RGB Video + CompositeSync out of it.

## What does it do, exactly?

Connects to a Raspberry PI 3(b) inside the housing of Arcadeblock(Nerdblock) Genesis USB Hub and turns it into a mini-videogame-system.
Video-Output is 15KHz-RGB. Needs configuration settings to output correct video. (Like/same as Pi2Scart or Pi2Jamma)
Uses the original USB-sockets from the USB-Hub's PCB.

## PCB Specs and getting hands on the boards
I can recommend itead.cc for pcb manufacturing. Either export the GERBER files from EAGLE using the files that I provided or wait until I finished writing this readme and find them inside the repository.
```
### PCB SPECS:
----------------
* 10.0 x 5.0 cm
* 1.2 mm Thickness
* Surface: HASL
```

### Installing

```
I made a PDF with an installation guide.
```
* desolder original USB-sockets and install them on the pcb
* solder PCB to GPIO-pins
* connect usb-pins with cables (D+ and D- Lines 1-4)
* connect usb-power-pin to one of the usb-sockets on the PI
* connect AUDIO from PI to SND-L and SND-R pins
* connect VIDEO-OUT to AV-Socket
* connect POWER and GND from PSU to 5V-IN
* connect POWER and GND from 5V-OUT to PI-Power-Input (miniUSB-port)
* when AUDIO has noise, use a groundloop-isolator between the connetction


## Additional Modding of the Hub's case

* DC-Power-Input (5V)
* Video-Out via 8-Pin-MiniDIN Socket (I also provided files for a convenient adapter)
* optional separate H- and V-Sync via dedicated cinch-sockets and cinch-to-bnc cables for studio monitors/PVM


## On the Software-Side

Search the web for GertVGA66, PI2SCART, PI2JAMMA and similar Projects. Once your PI is configured to output video through the GPIO port, the built-in DAC on the PCB will produce 15KHz RGB Video.



## Built With

* EAGLE (https://www.autodesk.de/products/eagle/overview)


## Versioning

This is likely the first and last release of this project.


## Authors

* **Alex Schütz**


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


## Acknowledgments

* This project is completely UNTESTED!
* Inspiration came from GERT/VGA666 and other Pi2RGB Projects
* Please don't mess with electronics if you have no clue what you're doing!


## Q&A's

* Why did you abandon this project?

• The USB-hubs are sold out and I have other stuff to care about.

* Why is the Raspberry Pi's sound so bad over the headphone jack?

• It's because of the PI's limitations regarding analogue sound. Get a USB-Soundcard! Those are dirtcheap and produce very acceptable audio.

* Can I still use HDMI as Video-Output?

• Sure, but then I suggest you just pass installing this pcb, it will not get you any advantage while using HDMI.

* Man, I love your stuff - Can you please send me a fully loaded pcb because I have 2 left hands and can't solder.

• Dude, just download the stuff that I release to the public. It usually contains everything you need to order PCBs wherever you want plus information on how to use or install it. Anyways, if you can't solder, sending you a pupulated PCB is like sending you a can, knowing you don't have a can-opener...
