# CATPAW_toolhead

CatPaw is the ideal toolhead for Voron Zero series with Orbiter 2.0 Extruder. I developped this toolhead as I was unhappy with the existing options. The standard Voron Zero 0.2 toolhead does not provide as much cooling as I prefer, and certinly less than the StealthBurner toolhead. My design goals were also minimum loss of print volume and maximum compatibillity with toolheads and options for probe and filament sensor.

CATPAW:
- Uses Voron Zero 0.2 toolhead cardridges, so should work with all toolheads for voron Zero 0.2 (fan saver reccomended)
- 2x 4010 Blowers, with StealthBurner duct layout for near arctic level part cooling (2x 4010 provides more air than StealthBurner toolhead)
- Allmost no loss in print volume. X axis should be full width, loss off a milimeter or so on X if you print with your door closed. (Magnets on my door are strong enough, so the door closes again if the toolhead bumps into it, giving me the full 120x120 mm even when printing ABS
- Option to add the slideswipe Probe. I shorteded the probe, but all other parts can be used from https://github.com/SaltyPaws/Voron_0.1and0.2mods/SlideSwipe or orignal repo (https://github.com/chestwood96/SlideSwipe)
- Option to add under extruder filament Sensor
- Carriages provided for MGN7 and MGN9 X-axis rails. It is reccomended to also print the provided X carriage for the appropriate rail. In order to minimize toolhead height, I lowered the screwhole for the rear mounting screw.
The toolhead will work with the stock Voron Zero 0.2 Carriage, but the screw securing the X-carriage from the rear will not fit.

<img src="https://github.com/SaltyPaws/CATPAW_toolhead/blob/main/images/PXL_20240101_224037977.jpg?raw=true" height="800" width="600" >

**BOM**
1. 2x NeoPixel
2. 1x 3010 hotend fan
3. 2x 4010 Blower
4. 6x3mm magnets for probe (optional)
5. 6mm steel ball for filament sensor (optional)
6. Omron D2F-L microswitch with lever for filament sensor (optional)
7. 2x M2x12 or selftapping screw to secure microswitch (optional)

# Installation Instructions
Assembly should be done in the follwing order:
**Probe**
- Solder wires to 6x3mm magnets. In order to prevent loss of magnetism, let the magnets cool against another 6x3 magnet.
- Press the magnets into the slots by pushing the toolhead down on a hard object.
- Use a large flat soldering tip at around 230C to push the magnets deeper into the slots, you want the magnets to stick out ~0.5 to 1 mm. Again, let the magnets cool down attached to oher magnets to prevent loss of magnetism.
- Ensure wire to magnet path has very low resistance (less than 4 ohm).
- route wires out torugh little side window.
- Seal hole with red gasket maker.

**NeoPixels**
- Create a chain of 2 neopixels. You do not have a lot of space to hide excess cable, so make the wires between the neopixels as short as possible, while still allowing them to slide into the slots.
- Test the neopixels! It will be more rework to remove the hotend fan and part cooling fans later.

**Fans**
- First install 3010 part cooling fan. Be very carefull to only press the edges of the fan, the fan will break when pushing the centre of the fan (ask me how I know...)
- Then proceed with intalling the blower fans.
- Use a knife to cut the upper right hand side of the blower fan (looking back to front). This is required for routing the majority of the wires, see pictures below:

<img src="https://github.com/SaltyPaws/CATPAW_toolhead/blob/main/images/PXL_20231225_175242278.jpg?raw=true" height="600" width="800" >

<img src="https://github.com/SaltyPaws/CATPAW_toolhead/blob/main/images/PXL_20231225_175256608.jpg?raw=true" height="800" width="600" >

<img src="https://github.com/SaltyPaws/CATPAW_toolhead/blob/main/images/PXL_20231225_175325632.jpg?raw=true" height="800" width="600" >
  
**Toolhead Cardridge**
- Ensure the heater wires are installed pointing towards the right hand fan that has space for wire routing.
- Thermistor, probe and fan wires will fit on the other side (left hand side fan).
- Hold off on installing the zip-ties, these are best installed after the toolhead is installed on the carriage.

**Filament Sensor**  
- Solder wires to filament sensor (2 othermost legs). You may want to shorten the legs somewhat for an easier fit.
- Trim lever, so that lever does not extend past microswitch body
- Install microswtich and ball
- Test sensor

**Install Toolhead**
- Carefully mount toolhead, ensuring that wires are not pinched, and belt is not rubbing on gantry. The bulk of the wires will go in the gap carved out on the right hand side fan, the other side will have sufficient space for probe and fan wires.
- 
**Min Probe**
- See installation instructions in orignal repo: https://github.com/chestwood96/SlideSwipe
