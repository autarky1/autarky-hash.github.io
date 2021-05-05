# Diana Tan

## Assignment 4
Part 1: Modify the mesh of two STLs to produce a single printable STL. You may use whatever STLs you want, e.g. downloaded from Thingiverse or elsewhere! When exporting the STL from Rhino, it should pass all checks for rapid prototyping.

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
Final: https://github.com/autarky-hash/autarky-hash.github.io/blob/main/DinoTardis.stl<p>
Original: https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Doctor_Who_Tardis.STL<p>
https://github.com/autarky-hash/autarky-hash.github.io/blob/main/dino.stl

## Part 2- Atlas Lamp

## Original STL Files
I selected 2 STL files I wanted to use for my lamp- 1 was a statue of Atlas (which originally came with its own earth). The earth that it came with though was a thin earth that required a different type of filament for the light to show through. I chose a different earth mesh that had a wireframe around it so that the light can shine through. 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/atlasearth.png" height=px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/wiredearth.png" height=px> 

Links:
<html> https://www.thingiverse.com/thing:4632906<p>
https://www.thingiverse.com/thing:175033<p></html>

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

## Adjusting the Mesh- Earth

1. I started by adjusting the earth mesh to the size of the light bulb. Because the light bulb is 100 mm, I needed to double the size of the earth which I did with the Scale command function to make the earth ~120mm. The main, issue with the earth, however was that the mesh was really bad. Basically, because the earth had a million different islands that were not going to print, I had to manually delete the meshes that were not going to work and run Repair Mesh multiple times to reconcile this. I converted the earth to NURBS. Even then, I don't think I got all of the islands out of the print.

2. I manually deleted all of the islands as much as I can and ran Repair Mesh multiple times until I got a Good Mesh. 

3. In order to create a hole to fit the light bulb, I needed to do a MeshBooleanDifference, which I did by creating a sphere the diameter of the widest width of the light bulb to carve a hole on the bottom. 

## Adjusting the Mesh- Atlas

4. I ran MeshtoNurbs on Atlas to change the surface to polysurfaces. I ran RepairMush multiple times and deleted some artifacts that was impacting the STL. However, I realized that the number of artifacts made it impossible to manually remove all of them. I kept running RepairMesh to see how many mesh surfaces were left.

5. I tried to scale Atlas accordingly on the bottom of the lamp. However, I realized that if I scaled Atlas to be as big as the globe, it would exceed the build height of my printer. Instead, I scaled Atlas a little to hold the earth up at the lowest point and then duplicated him to make 2 supports on the bottom. I did a "Mirror" command on the 2nd Atlas structure so that it faced the opposite direction.

6. I used distance to measure the distance between Atlas to see if it can fit the bottom of the lamp and then tried to move it up so that it would intersect with the globe.

7. I did MeshBooleanunion to combine Atlas and Earth.

<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoAtlaslamp.png" height=px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoAtlaslamp2.png" height=px> 

## Printing the Lamp


8.  
9. 

7. 

