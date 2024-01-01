# CATPAW_toolhead

CatPaw is the ideal toolhead for Voron Zero series with Orbiter 2.0 Extruder. I developped this toolhead as I was unhappy with the existing options. The standard Voron Zero 0.2 toolhead does not provide as much cooling as I prefer, and certinly less than the StealthBurner toolhead. My design goals were also minimum loss of print volume and maximum compatibillity with toolheads and options for probe and filament sensor.

CATPAW:
- Uses Voron Zero 0.2 toolhead cardridges, so should work with all toolheads for voron Zero 0.2 (fan saver reccomended)
- 2x 4010 Blowers, with StealthBurner duct layout for near arctic level part cooling (2x 4010 provides more air than StealthBurner toolhead)
- Allmost no loss in print volume. X axis should be full width, loss off a milimeter or so on X if you print with your door closed. (Magnets on my door are strong enough, so the door closes again if the toolhead bumps into it, giving me the full 120x120 mm even when printing ABS
- Option to add the slideswipe Probe. I shorteded the probe, but all other parts can be used from orignal repo (https://github.com/chestwood96/SlideSwipe)
- Option to add under extruder filament Sensor
- Carriages provided for MGN7 and MGN9 X-axis rails. It is reccomended to also print the provided X carriage for the appropriate rail. In order to minimize toolhead height, I lowered the screwhole for the rear mounting screw.
The toolhead will work with the stock Voron Zero 0.2 Carriage, but the screw securing the X-carriage from the rear will not fit.

<img src="https://github.com/SaltyPaws/CATPAW_toolhead/blob/main/images/PXL_20240101_224037977.jpg?raw=true" height="800" width="600" >

# Installation Instructions
**Probe**
Start with assembling the probe magnets. For best result I like to:
- Solder wires to 6x3mm magnets. In order to prevent loss of magnetism, let the magnets cool against another 6x3 magnet.
- Press the magnets into the slots by pushing the toolhead down on a hard object.
- Use a large flat soldering tip at around 230C to push the magnets deeper into the slots, you want the magnets to stick out ~0.5 to 1 mm. Again, let the magnets cool down attached to oher magnets to prevent loss of magnetism.
- Ensure wire to magnet path has very low resistance (less than 4 ohm).
- route wires out torugh little side window.
- Seal hole with red gasket maker.

**NeoPixels**
- Create a chain of 2 neopixels. You do not have a lot of space to hide excess cable, so make the wires between the neopixels as short as possible, while still allowing them to slide into the slots.
- Test the neopixels! It will be more rework to remove the hotend fan and part cooling fans later.

- 
