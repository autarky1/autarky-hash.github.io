# Diana Tan

## Part 1: Modify the mesh of two STLs to produce a single printable STL. You may use whatever STLs you want, e.g. downloaded from Thingiverse or elsewhere! When exporting the STL from Rhino, it should pass all checks for rapid prototyping.

Part 2: Please make (a start on) a lamp! Using your lamp innereds' measurements as a point of departure, make a lamp that can be assembled around the innereds out of 3D printed parts. You should be able to remove the lamp from the innereds again, so you cannot attach the lamp to the innereds with glue, fasteners, adhesive, etc. This will require you to think carefully about the interface between your parts. Imagine your lamp being in a domestic setting---perhaps it will not be wildly shaken, but it should not fall apart with normal use. For the rest of the lamp, get creative!

Documentation for this assignment: Document your project on a webpage linked to from your main webpage. You will be expected to talk about your project in class next week using your webpage documentation as your presentation material. We want to know about what your lamp plan is, and how you are progressing through design, CAD, and printing. 

## Part 1- Dino Tardis

## Find 2 STLs
First I found 2 STLs on thingiverse to make a lamp out of. 
Dino: https://www.thingiverse.com/thing:913069/files
Tardis: https://www.thingiverse.com/thing:153977

## Check Mesh
I checked the mesh of the dino by using Repair Mesh. It said "good mesh". Then I tried to do ReduceMesh but I found that the dino only has 650 polygons.
I checked the mesh of the Tardis by using Repair Mesh. It also said good mesh. The Tardis had 40,302 polygons so I did ReduceMesh to switch it to 10,000 polygons.
I also then did a MeshToNURB on both meshes to get them to turn into polysurfaces.
<img src= "https://github.com/autarky-hash/autarky-hash.github.io/blob/main/GoodMesh.png" height=px>

## Scale & Halve Dino

I did a ScaleMesh on the Tardis so that the height would match the lamp. Then I actually did a plane against the Tardis and a solid plane against the Dino to carve out half of each shape. I did a MeshBooleanDifference against the Tardis and the plane and then the plane against the Dino. I also then did a MeshBoolean DIfference against the Tardis vs. the Dino to place the Tardis inside of the Dino. This resulted in a closed mesh of both the Tardis and the Dino. 

Finally, I did a MeshBooleanUnion of the Dino and Tardis to embed the Tardis inside the Dino. This created a single mesh of both shapes. 

## Dino Tardis
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/DinoTardis2.png" height=px> 
<img src= "https://github.com/autarky-hash/autarky-hash.github.io/blob/main/DinosaurTardisRhino.png" height=px>
</html>

## STL Files
Original:
Final:

## Part 2- Atlas Lamp

## Original STL Files
I selected 2 STL files I wanted to use for my lamp- 1 was a statue of Atlas (which originally came with its own earth). The earth that it came with though was a thin earth that required a different type of filament for the light to show through. I chose a different earth mesh that had a wireframe around it so that the light can shine through. 

Links:
https://www.thingiverse.com/thing:4632906
https://www.thingiverse.com/thing:1750333

## Measuring the Lamp Base
I measured the lamp innerds with my calipers. 
Widest part of the light bulb: 65 mm
Width of the Light Bulb touching connector: 31.09 mm
Length of the Light Bulb: 100 mm
Length of Connector: 58.77 mm
Width of Light Bulb Connector: 37.15 mm
Width of the Light Bulb Wire: 3.15 mm

## Checking the Mesh of STL Files
I checked the mesh of both the STL files and they were both bad meshes with Repair Mesh. The Atlas statue had a whopping 194k polygons while the Earth had 50k polygons. I did a Reduce Mesh on both files so that each had ~20k polygons. On top of that, the earth mesh was not manifold and had a lot of disjointed parts because I think someone took a globe and overlaid it against a sphere. 

## Adjusting the Mesh

1. I started by adjusting the earth mesh to the size of the light bulb. Because the light bulb is 100 mm, I needed to double the size of the earth which I did with the scale function to make the earth ~120mm. The main, issue with the earth, however was that the mesh was really bad. Basically, because the earth had a million different islands that were not going to print, I had to manually delete the meshes that were not going to work and run Repair Mesh multiple times to reconcile this. I converted the earth to NURBS. Even then, I don't think I got all of the islands out of the print.

2. In order to create a hole to fit the light bulb, I needed to do a MeshBooleanDifference, which I did by creating a sphere the diameter of the widest width of the light bulb to carve a hole on the bottom.   




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

