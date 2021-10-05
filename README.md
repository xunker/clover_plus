My custom CloverPlus 3D printer
===============================

<!-- vscode-markdown-toc -->
* 1. [Marlin Config](#MarlinConfig)
* 2. [Printed Parts](#PrintedParts)
	* 2.1. [Chassis](#Chassis)
	* 2.2. [Carriages](#Carriages)
	* 2.3. [Bed clamps](#Bedclamps)
	* 2.4. [Effector and collar](#Effectorandcollar)
	* 2.5. [Filament Spool](#FilamentSpool)
	* 2.6. [Display Case](#DisplayCase)
	* 2.7. [RAMPS case](#RAMPScase)
	* 2.8. [Z-Axis Brace](#Z-AxisBrace)
* 3. [Non-printed bits](#Non-printedbits)
	* 3.1. [Rods](#Rods)
	* 3.2. [Bearings](#Bearings)
	* 3.3. [Extruder](#Extruder)
	* 3.4. [Power Supply and electronics](#PowerSupplyandelectronics)
	* 3.5. [Delta Arms](#DeltaArms)
	* 3.6. [Glass Bed](#GlassBed)
	* 3.7. [Hot end](#Hotend)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

My custom CloverPlus 3D printer
===============================

In May 2016 I started to build my own 3D printer (using one I already had, as you do). The design I chose was called "CloverPlus".

After a shaky start, it became my main 3D printer. Reasons included it was much smaller than my Robo3D printer, and (after tuning) it was much more accurate as well.

This repo is a clearinghouse of everything about that printer so you can build one if you want, but mostly so I have a place to put things so they won't get lost.

"Make" on thingiverse: https://www.thingiverse.com/make:208007

##  1. <a name='MarlinConfig'></a>Marlin Config

I'm still using an ancient build of Marlin (1.1.0 RC5) on an ancient RAMPS clone, but it works just fine. You can find details of my Marlin config on [MARLIN.md](MARLIN.md).

##  2. <a name='PrintedParts'></a>Printed Parts

My printer is a hodge-podge of parts from different versions, parts that just fit, or parts I've designed myself.

###  2.1. <a name='Chassis'></a>Chassis

The main upper and lower chassis pieces are from [CloverPlus v2](https://www.thingiverse.com/thing:1374313).

###  2.2. <a name='Carriages'></a>Carriages

Using the Z carriages from [Mystereon's V2](https://www.thingiverse.com/thing:2102151), but not using optical endstops.

###  2.3. <a name='Bedclamps'></a>Bed clamps

Clamps from [CloverPlus v2](https://www.thingiverse.com/thing:1374313).

###  2.4. <a name='Effectorandcollar'></a>Effector and collar

Effector is some random Kossel Mini effector, can't remember the source. Collar is, I think, a [Mini Kossel groove mount](https://www.thingiverse.com/thing:108023).

###  2.5. <a name='FilamentSpool'></a>Filament Spool

[Quick Change Universal Spool Holder](https://www.thingiverse.com/thing:1241566), on a long piece of old 5/16th rod and attached to the top of the printer using a pair of [any-angle rod clamps](https://www.thingiverse.com/thing:30328).

###  2.6. <a name='DisplayCase'></a>Display Case

Case for the RepRap Discount display is the [Case for the Full Graphic Smart LCD Controller](https://www.thingiverse.com/thing:87250).

###  2.7. <a name='RAMPScase'></a>RAMPS case

The case for the RAMPS electronics is [Dasaki Ramps 1.4 Enclosure / Box / Case](https://www.thingiverse.com/thing:761806).

###  2.8. <a name='Z-AxisBrace'></a>Z-Axis Brace

The [CloverPlus Smooth Rod Brace](https://www.thingiverse.com/thing:4982844), designed by me to reduce z-axis sway.

##  3. <a name='Non-printedbits'></a>Non-printed bits

###  3.1. <a name='Rods'></a>Rods

Although I started the design using 5/16 smooth rod, I quickly came to my senses and switched to standard 8mm smooth rod.

###  3.2. <a name='Bearings'></a>Bearings

Standard LM8UU bearings.

###  3.3. <a name='Extruder'></a>Extruder

Some MK8 kockoff from Amazon, connected to a beefy (but ungeared) stepper.

###  3.4. <a name='PowerSupplyandelectronics'></a>Power Supply and electronics

Power supply is an old XBox 360 PS from a second-hand store. Control hardware is basic RAMPS 1.4 setup (Bigtreetech I think).

###  3.5. <a name='DeltaArms'></a>Delta Arms

Some random 217mm carbon fiber arms, I can't remember where from. I should use shorter arms, but these were cheaper at the time.

###  3.6. <a name='GlassBed'></a>Glass Bed

Some random 120mm (3mm thick) borosilicate plate. Previously I was using a 7-inch round mirror from a craft store.

###  3.7. <a name='Hotend'></a>Hot end

Some random V6-clone from eBay. Cooling is currently handled by a [Haldis cooling shroud](https://www.amazon.com/dp/B08Z713MSK).

