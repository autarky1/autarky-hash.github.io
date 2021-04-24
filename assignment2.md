# Diana Tan

## Assignment 2: Getting Started with 3D Printer
Assemble your 3D printer and document the process on your website. Include the following steps:
First, conduct the bed leveling protocol from Filament Friday: https://www.thingiverse.com/thing:3235018 (Links to an external site.)
Once your bed is well leveled, print the following test prints:
A 2cm cube with the standard "low quality" settings 
A 2cm cube with the standard "standard quality" settings 
A 2cm cube with the standard "super quality" settings
If you are having adhesion issues, we recommend slowing down the initial layer to half speed and/or  try using a "BRIM" for build plat adhesion.
A 2 cm cube with a concentric top and bottom layer and your favorite print setting from the previous cubes.
Next, we will print tubes: 

A tube 3cm in diameter and 3cm high with a single extrusion wall thickness
A tube 3cm in diameter and 3cm high with a double extrusion wall thickness and random z-seam alignment
A cylinder 3cm in diameter exported with a 0.1mm tolerance
A cylinder 3cm in diameter exported with a 0.001mm tolerance
A cylinder 3cm in diameter with special mode "spiralize outer contour".
A cylinder 3cm in diameter printed on its side with supports on.
For each of these prints, document how long they took, and measure their height/width with calipers and and document their sizes. 

20.0mm +/- 0.1mm cube with a 10.0mm +/- 0.1mm hole through it.
To do this, you will need to calibrate your print settings by measuring output from your printer with your calipers. It is likely you will have to print this several times to get it to tolerance!
## Step 1: Assemble Printer (6 hours!)
Due to the fact that my printer arrived many days later and I had to resort to Amazon Prime the day before the assignment is due, I first spent many hours assembling the printer, making sure that the screws were tightened, filament was inserted and that the connections were correct. The most complex part of this process was actually trying to understand why the printer did not turn on- which I found from the slide deck (and not in the printer instructions) was due to moving the switch in the back to a different voltage with a screw driver. A huge learning was also in the fact that  also in the movement of the cables which got in the way of the printer. 

## Step 2: Level Plate
I leveled the plate in 2 different ways- one with a piece of paper manually and then moving the knobs underneath the printer until the filament touched the plate. I also did this again with the bed leveling protocol from Filament Friday by loading the files onto the SD card and then onto the machine.

## ERROR! Homing Failed
I got stuck on homing failed on the machine, Please reset multiple times. Sometimes I manage to exit the error by turning the machine on and off again or by moving the printer head or by moving the cables I always inevitably ended up back at Homing Failed.

## ERROR! Leveling Print in 1 Line
I tried to create a leveling print with the Filament Friday leveling file but instead the printer only moved on 1 axis repeatedly and created a straight line. After I started the print, the printer didn't show an error but also didn't move in the square box that was in the video.

## ERROR! Nozzle Stuck
After the printing in 1 line, the printer then printed on itself repeatedly until the nozzle got stuck. Thanks our class Discord, Kenny (shoutout!) told me to heat up the PLA which released the misprint. 

## MANY HOURS LATER (24+ hours later)
I realized that my error many hours later was in the initial assembly of the printer itself- I did not realize that there was a roll for the belt behind the QR code for the Ender Pro. Because of that, my y did not align and it would not auto home. I had tried everything- attempting to level and level, tightening it manually, trying to unplug all of hte plugs and replugging them. After I tightened the belt, I was able to finally level the plate.

## Step 3: Rhino Model- Cube Test Print
I created a Rhino Model of the cube first through the Solid -> Cube function. I used a mm function and also created a solid box for the maker itself under 220mmx220mmx250mm.

## Step 4: Import Rhino Cube into Ultimaker Cura
I then placed my cube into Ultimaker Cura. In Ultimaker, I managed to set the cube quality from low to high. However, the time greatly varied. The Low quality cube was reported to take 20 minutes, the standard quality cube was reported to take 26 min and slicing for a high quality cube was reported to take 33 min.

## Step 5: Printing my First Cube (6+ hours)
I loaded my cubes into Ultimaker and ran into a series of issues, mostly regarding adhesion

## Step XX:
I rotated the cylinder on its side by going into Snap Rotation and moving the cylinder.

## Step xx: Checking Calipers
First I turned on the calipers by clicking on the on switch and then zeroing it out and setting it to the origin.
Then I did my outer management by putting the objects in the jaws, followed by the inner measurements. Here are my results:


## Step 4: Rhino Files (for Reference)
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoCube.3dm
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoCylinder.3dm

