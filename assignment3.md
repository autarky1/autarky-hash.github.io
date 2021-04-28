# Diana Tan

## Part 1: Making a construction kit

Create a grasshopper definition of a clip and 3D print the clip. Your clip should allow you to connect a piece of cardboard to another piece of cardboard. Your grasshopper definition should allow you to vary the thickness of the cardboard. Print at least 10 clips and clip pieces of cardboard together with them. If you pick up your clipped together cardboard and shake it, it should not fall apart! Submit the grasshopper definition, your STL, and a video of you shaking your construction.

## Grasshopper Definition
First I created a grasshopper definition of the clip which allowed me to vary the amount of inputs and outputs so that I can manipulate the array. I created a circle, rectangle, and polar arrays with input for slot depth, slot width and number of slots. Then, I baked the shapes as I played around with them in Rhino.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Grasshopper.png" height=px> </html>

## Rhino Shapes
Then I went from grasshopper back to Rhino to move the shape out and then did a curve boolean to remove the excess. After I did the curve boolean, I removed the remaining bits by just cutting and deleting and then I extruded the curve. I printed 10 clips of varying levels of width, depth and height based on changing the settings in grasshopper. 

## Printing 10 Clips
I documented the print settings of each print. I initially tried to print all 10 paper clips simultaneously but then decided that the prints go faster if I did them one at a time so I have mutliple STL files.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/PaperclipSettings.png" height=px> </html>
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/IMG_1013.JPG" height=px> </html>

## Video
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/IMG_1016.MOV" height=px> </html>

## STL File


## Part 2: Making nested objects

Create a grasshopper definition that creates nesting structures (E.g. using offsets) that can be 3D printed in their nested state. You should have at least 3 nesting structures. Bake the result, export an STL, and 3D print the nested structure. The geometry can be whatever you want. Submit the rhino file, the grasshopper definition, your STL, and documentation of the print.

## Grasshopper Setting
I started by creating a Polygon in Grasshopper with a number slider. I then did an offset of the polygon multiple times.
<html><img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Grasshopper2.png" height=px> </html>

## Rhino Setting
When I went into Rhino, I did Curve Boolean again and extracted the curves of my pentagon. I then deleted the excess layers and then extruded the curve. However, I noticed that i had multiple mesh issues when I imported the file into Ultimaker Cura. I had to keep going back into Rhino to edit the file.

## Nested Print
I managed to finally make the nested print. I used a brim on the bottom of the print of the pentagon.

## STL File
