# Pico360 Harness
#### A custom and more professional Harness for the PicoFlasher
##### Prerelease 0.0.1
Kevin Karhan et. al.

---
## FAQs
### Why did you make this?

I wanted to mod multiple Xbox 360 Slim & Slim-E that I got for a bargain in one go, so I wanted to avoid having to desolder anything and make that experience as plug and play as possible.

Since [RGH3 doesn't require any expensive and/or out-of-production modchip](https://gbatemp.net/threads/reset-glitch-hack-3-rgh3-for-xbox-360-with-instant-boot.606307/) but instead builds a custom NAND signed with the per-device unique console key, it'll basically result in an instant-booting 360.

#### Basically, instead of soldering and desoldering a bunch of probe pins every time, I decided to only solder / stick in what I can't reasonably remove and instead install some 2,54mm pin plugs.

Furthermore, I wanted a more elegant way to [dis]connect stuff that is more in line with a professional tool and allows me to undo the work if need be.

### What one will still need to install and solder on their Xbox 360:
- The necessary bottom wires
  - Use 0,05mm² aka. "30 AWG" solid core for best results.
  - Including the appropriate resistor
    -  1 kΩ on "Corona" mainboards
    - 10 kΩ on "Trinity" mainboards
  - The "Postfix Adaptor"
    - Some people claim to be able to solder diectly to that XCGPU pin, but if you're that kind of person, than you don't want or need this adaptor anyway.
      - At [U$D 3,75 per piece](https://weekendmodder.com/store/index.php?route=product/product&path=60&product_id=148) it's not worth the time and risk of any professional installer...
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
    - Yes I also know that the [PC2NEO USB](http://unibios.free.fr/pc2neo.html) looks similar but it's safe to assume these won't get mixed together
- I could've used a ["RJ-50" 10p10c](https://en.wikipedia.org/wiki/Modular_connector#10P10C) connector if I put all the GND lines together, but not only are they even harder to find at a reasonable price, but some people may attempt to violently shove it into an RJ-45 Ethernet socket anyway.
  - Also I don't want to fiddle with said tiny connectors when I can get DA-15 terminal blocks & plug casings for less than the tooling needed to properly crimp 10P10C connectors.
    - I can put the PicoFlasher in the same case as the adaptor and basically have a clean setup - at least from the outside.
---
## Acknowledgements
### Projects
- [X360Tools Project](https://github.com/X360Tools)
  - [PicoFlasher](https://github.com/X360Tools/PicoFlasher)
  - [JRunner Pro](https://github.com/X360Tools/J-Runner-Pro)
  - [XeLL-Reloaded](https://github.com/X360Tools/xell-reloaded)
### Writeups
- [The WeekendModder](https://www.weekendmodder.com/index.html)
  - [PicoFlasher Info](https://www.weekendmodder.com/picoflasher.html)
- [xXBeefyDjXx's writeup on RGH3](https://www.se7ensins.com/forums/threads/rgh-3-0-guide-phat-slim-includes-quick-tool.1832979/)
### Videos
- [15432](https://www.youtube.com/@alexs.6892)
  - [Xbox 360 RGH3 Demo](https://www.youtube.com/watch?v=iVYqxLZ_KL0)
  - [Xbox 360 - RGH3 Installation?](https://www.youtube.com/watch?v=21HAn1-zwLg)
- [MrMario2011](https://mistermario.net/)'s excellent step-by-step Tutorials
  - [How to RGH3 a Xbox 360 Slim (Trinity) - Chipless RGH 3.0 Tutorial!](https://www.youtube.com/watch?v=D3DDglRBqfY)
  - [How to RGH3 a Xbox 360 Slim (Corona) - Chipless RGH 3.0 Tutorial!](https://www.youtube.com/watch?v=hpOlGeCHwro)
- [Modern Vintage Gamer](https://www.youtube.com/@ModernVintageGamer) - in case you need some convincing on why you should mod your Xbox 360 as someone who only plays single-player / splitscreen or LAN multiplayer and don't want to use Xbox Live at all.
  - [Why YOU need a Modded Xbox 360 in 2018](https://www.youtube.com/watch?v=8gduINQMxd0)
  - [The Xbox 360 is still awesome in 2019](https://www.youtube.com/watch?v=zFGz4aT1cgo)
  - [Revisiting Original Xbox Backward Compatibility on the Xbox 360 - Run ALL Original Xbox Games](https://www.youtube.com/watch?v=Da_ont-2AG0)
### Products
- [Raspberry Pi](https://www.raspberrypi.com/)
  - [RP2040](https://www.raspberrypi.com/products/rp2040/)
    - [Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/)
- [The WeekendModder Shop](https://weekendmodder.com/store/index.php)
  - [PicoFlasher Custom Cable Harness](https://weekendmodder.com/store/index.php?route=product/product&path=60&product_id=274)
    - I got inspired by this and the [Universe BIOS's](http://unibios.free.fr/index.html) [PC2Neo Cable](http://unibios.free.fr/pc2neo.html).
