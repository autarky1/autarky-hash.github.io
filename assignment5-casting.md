# Diana Tan

## Assignment 5 (Part 2!)

<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoAtlaslamp.png" height=px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/RhinoAtlaslamp2.png" height=px> 

## Part 2: Casting/Beginning of Final Project

Intro: I wanted to create bike trophies for my work team (I work on delivery bikes). The bike that we used is custom manufactured so there is no STL file readily available. I also wanted to make an assortment of other bikes for my co-workers themed after things they worked on as well.

## Photoshop/AI Edit: 
I actually started by tracing the (grainy) bike model of the file that we had at work. I took the initial photo and colored in black and white to omit the detail. I also deleted some detail I didn't want (like small text), wheels, etc.
In Illustrator, I did an image trace and then cleaned up stuff like curves in detail, making some curves wider so that it would be easier to print.

## Rhino Mold:
In Rhino, I imported the AI file and then extruded the model of the bike. Then I turned on Draft Angle Analysis to be able to see all surfaces.

## Side 1:
I then broke up the bike into 3 poly surfaces per side. For the more complex side, it was actually relatively straightforward- I exploded the polysurface and then offset the curve. Junchao helped me then edit the curves (BlendCurve, CloseCurve) and also use Loft so that it would actually create a planar surface. I flipped the model several times until I was able to get a good planar surface. I then did a Blend Surface betwen the 2 outer layers of the plane. 

I then trimmed the outer layer of the planar surface to create a square that I can then extrude into the outer layers of my mold.

## Side 2: 
This was an absolutely painful experience. I exploded the polysurface but the lines of the mold intersected and did not sit on a planar surface. Because of the shape of the object, Junchao helped me edit the curves (BlendCurve, Close Curve) But because the object existed in its own 3D dimension, it will not form a planar surface for me to make the mold out of. Instead, what I actually ended up doing was offsetting the curves and then lofting the curve and scaling it multiple times instead instead. Then, I actually, created a "shell" by using "steep1" in Rhino instead and formed a sort of outer layer for the curve so that it will sort-of form a planar surface.  
