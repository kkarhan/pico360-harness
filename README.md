# Pico360 Harness
#### A custom and more professional Harness for the PicoFlasher
##### Prerelease 0.0.1
Kevin Karhan et. al.

---
## FAQs
### Why did you make this?

I do want to mod multiple Xbox 360 Slim that I got for a bargain in one go, so I wanted to avoid having to desolder anything and make that experience as plug and play as possible.

#### Basically, instead of soldering and desoldering a bunch of probe pins every time, I decided to only solder/stick in what I can't reasonably remove and instead install some 2,54mm pin plugs.

Furthermore, I wanted a more elegant way to [dis]connect stuff that is more in line with a professional tool and allows me to undo the work if need be.

### What one will still need to install and solder on their Xbox 360:
- The necessary bottom wires
  - Use 0,05mm² aka. "30 AWG" solid core for best results.
  - Including the appropriate resistor
    -  1 kΩ on "Corona" mainboards
    - 10 kΩ on "Trinity" mainboards
  - The "Postfix Adaptor"
    - Some people claim to be able to solder diectly to that XCGPU pin, but if you're that kind of person, than you don't want or need this adaptor anyway.
- 2,54mm pin header jacks

### Why would anyone want to do this?
#### Instead of having some "ugly wiring" this will inevitably make it easier to just setup stuff.

### Why did you choose the connectors you chose to do this?
#### Short answer: It looks more professional.
- It is necessary to unplug the Programmer to restart the console, so [having just one connection to disconnect is faster and easier.](https://youtu.be/hpOlGeCHwro?t=4654)
- I want to avoid desoldering unless I fucked up soldering.
#### Long Answer: To idiot-proof the tooling!
- The [DA-15 connector](https://en.wikipedia.org/wiki/D-subminiature#Description,_nomenclature,_and_variants) - unlike the [VGA-Connector](https://en.wikipedia.org/wiki/VGA_connector) - is quite uncommon and won't fit in neither VGA nor [RS-232](https://en.wikipedia.org/wiki/RS-232#Data_and_control_signals) connectors.
  - Yes I know it's the same connector as the [Gameport](https://en.wikipedia.org/wiki/Game_port) [used](https://en.wikipedia.org/wiki/D-subminiature#DA-15_connectors_2) and the [Apple IIc & IIe Display](https://en.wikipedia.org/wiki/D-subminiature#DA-15_connectors) but if you think those belong hooked up to an Xbox 360 then maybe you should not be allowed to touch anything more complex than a light switch and a "stupid phone" with a number pad.
- I could've used a ["RJ-50" 10p10c](https://en.wikipedia.org/wiki/Modular_connector#10P10C) connector if I put all the GND lines together, but not only are they even harder to find at a reasonable price, but some people may attempt to violently shove it into an RJ-45 Ethernet socket anyway.
- I can put the PicoFlasher in the same case as the adaptor and basically have a clean setup.
---
## Acknowledgements
### Projects
- [X360Tools Project](https://github.com/X360Tools)
  - [PicoFlasher](https://github.com/X360Tools/PicoFlasher)
### Writeups
- [The WeekendModder](https://www.weekendmodder.com/index.html)
  - [PicoFlasher Info](https://www.weekendmodder.com/picoflasher.html)
### Videos
- [15432](https://www.youtube.com/@alexs.6892)
  - [Xbox 360 RGH3 Demo](https://www.youtube.com/watch?v=iVYqxLZ_KL0)
  - [Xbox 360 - RGH3 Installation?](https://www.youtube.com/watch?v=21HAn1-zwLg)
- [MrMario2011](https://mistermario.net/)'s Tutorials where he does excellent step-by-step tutorials
  - [How to RGH3 a Xbox 360 Slim (Trinity) - Chipless RGH 3.0 Tutorial!](https://www.youtube.com/watch?v=D3DDglRBqfY)
  - [How to RGH3 a Xbox 360 Slim (Corona) - Chipless RGH 3.0 Tutorial!](https://www.youtube.com/watch?v=hpOlGeCHwro)
### Products
- [Raspberry Pi](https://www.raspberrypi.com/)
  - [RP2040](https://www.raspberrypi.com/products/rp2040/)
    - [Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/)
- [The WeekendModder Shop](https://weekendmodder.com/store/index.php)
  - [PicoFlasher Custom Cable Harness](https://weekendmodder.com/store/index.php?route=product/product&path=60&product_id=274)
