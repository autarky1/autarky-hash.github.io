# Diana Tan

## Part 1: Modify the mesh of two STLs to produce a single printable STL. You may use whatever STLs you want, e.g. downloaded from Thingiverse or elsewhere! When exporting the STL from Rhino, it should pass all checks for rapid prototyping.

Part 2: Please make (a start on) a lamp! Using your lamp innereds' measurements as a point of departure, make a lamp that can be assembled around the innereds out of 3D printed parts. You should be able to remove the lamp from the innereds again, so you cannot attach the lamp to the innereds with glue, fasteners, adhesive, etc. This will require you to think carefully about the interface between your parts. Imagine your lamp being in a domestic setting---perhaps it will not be wildly shaken, but it should not fall apart with normal use. For the rest of the lamp, get creative!

Documentation for this assignment: Document your project on a webpage linked to from your main webpage. You will be expected to talk about your project in class next week using your webpage documentation as your presentation material. We want to know about what your lamp plan is, and how you are progressing through design, CAD, and printing. 

## Part 1-

## Find 2 STLs
First I found 2 STLs on thingiverse to make a lamp out of. 
Dino: https://www.thingiverse.com/thing:913069/files
Tardis: https://www.thingiverse.com/thing:153977

## Check Mesh
I checked the mesh of the dino by using Repair Mesh. It said "good mesh". Then I tried to do ReduceMesh but I found that the dino only has 650 polygons.
I checked the mesh of the Tardis by using Repair Mesh. It also said good mesh. The Tardis had 40,302 polygons so I did ReduceMesh to switch it to 10,000 polygons.
I also then did a MeshToNURB on both meshes to get them to turn into polysurfaces.

## Scale & Halve Dino

I did a ScaleMesh on the Tardis so that the height would match the lamp. Then I actually did a plane against the Tardis and a solid plane against the Dino to carve out half of each shape. I did a MeshBooleanDifference against the Tardis and the plane and then the plane against the Dino. I also then did a MeshBoolean DIfference against the Tardis vs. the Dino to place the Tardis inside of the Dino. This resulted in a closed mesh of both the Tardis and the Dino. 

Finally, I did a MeshBooleanUnion of the Dino and Tardis to embed the Tardis inside the Dino. This created a single mesh of both shapes. 


## STL Files
Original:
Final:

## Part 2-


https://www.thingiverse.com/thing:4632906

https://www.thingiverse.com/thing:2356344
https://www.thingiverse.com/thing:3348182
https://www.thingiverse.com/thing:3349700


<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Grasshopper.png" height=px> </html>

## Measuring the Lamp Base
I measured the lamp innerds with my calipers. 
Widest part of the light bulb: 65 mm
Width of the Light Bulb touching connector: 31.09 mm
Length of the Light Bulb + : 100 mm
Length of Connector: 58.77 mm
Width of Light Bulb Connector: 37.15 mm
Width of the Light Bulb Wire: 3.15 mm

## Rhino Shapes
Then I went from grasshopper back to Rhino to move the shape out and then did a curve boolean to remove the excess. After I did the curve boolean, I removed the remaining bits by just cutting and deleting and then I extruded the curve. I printed 10 clips of varying levels of width, depth and height based on changing the settings in grasshopper. 

## Printing 10 Clips
I documented the print settings of each print. I initially tried to print all 10 paper clips simultaneously but then decided that the prints go faster if I did them one at a time so I have mutliple STL files.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/PaperclipSettings.png" height=px> </html>
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/IMG_1013.JPG" height=px> </html>

## Video
Link https://drive.google.com/file/d/1TZHVffnY4FFO1f2AdLM7L6f6nrV5j5PF/view?usp=sharing

## STL File
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/1Clip.stl
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/2Clip.stl
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/3Clip.stl
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/4Clip.stl
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/5Clip.stl
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/6-9Clip.stl


## Part 2: Making nested objects

Create a grasshopper definition that creates nesting structures (E.g. using offsets) that can be 3D printed in their nested state. You should have at least 3 nesting structures. Bake the result, export an STL, and 3D print the nested structure. The geometry can be whatever you want. Submit the rhino file, the grasshopper definition, your STL, and documentation of the print.

## Grasshopper Setting
I started by creating a Polygon in Grasshopper with a number slider. I then did an offset of the polygon multiple times.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Grasshopper2.png" height=px> </html>

## Rhino Setting
When I went into Rhino, I did Curve Boolean again and extracted the curves of my pentagon. I then deleted the excess layers and then extruded the curve. However, I noticed that i had multiple mesh issues when I imported the file into Ultimaker Cura. I had to keep going back into Rhino to edit the file.

## Nested Print
I managed to finally make the nested print. I used a brim on the bottom of the print of the pentagon.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/IMG_1012.JPG" height=px> </html>


## STL File
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/NestedShapes3.stl

## Rhino Files
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/NestedShapes.3dm
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/PaperClips.3dm

