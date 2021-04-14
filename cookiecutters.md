# Diana Tan

## Assignment 1: My First Rhino Model!
Using Rhino, create 3 different "cookie cutter" (like these: https://www.treelittletree.com/maple-leaf-cookie-cutter.html (Links to an external site.)) shapes, and export them as STLs. Your cookie cutters should be a reasonable cookie size, e.g. between 1 and 6 inches. Your shapes have to come from images, i.e. you must create curves in illustrator or some other program and import them into Rhino, then build a solid model using those curves. Each STL must contain only one surface, which should not self-intersect or have other discontinuities. Document your process on your webpage, linking to your rhino model, your STLs, and your original image source files.
FAQ!
Q: Do I have to use Rhino? A: Yes
Q: Do I have to use Illustrator? A: No, you may also use other programs for image and vector manipulation such as Inkscape or Gimp.
Q: Can I use an svg/ai/existing vector file to make my shapes? A: No, you must generate your geometry from an image.
Q: Do I have to make the image myself or can I use existing images? A: You can use whatever images, as long as you give the original image creators attribution.
Q: Do I have to use github? A: Yes! You must include documentation and source files linked to from your github hosted webpage.
## Step 1: Photo Selection
I originally chose the following photos: <p>
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/pexels-anna-shvets-4587992.jpg" height=250px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/pexels-prasanth-inturi-1051838.jpg" height=250px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/pexels-anastasiya-gepp-1984437.jpg" height=250px> 
<p> 1. Attribution: Anna Shvets @ Pexels <a href="https://www.pexels.com/photo/cute-dog-wearing-a-party-hat-4587992/"> Link</a>
<p> 2. Attribution: Prasanth Inturi @ Pexels <a href="https://www.pexels.com/photo/silhouette-of-man-at-daytime-1051838/"> Link</a>
<p> 3. Attribution: Anastasiya Gepp @ Pexels <a href="https://www.pexels.com/photo/photo-of-woman-raising-her-both-hands-1984437/"> Link</a></p>

## Step 2: Background Removal & Image Tracing in Photoshop and Illustrator
I removed the background in Photoshop of each photo, converted the photo to black and white with high contrast, put the photos into gaussian blur and then thresholded the photo. I cropped the photos to relevant parts and then imported the files to Illustrator where I then did an image trace. After image trace, I meticulously removed artifacts, smoothed the points and reconciled any additional image issues. I also removed the fill and added a stroke to each image so that the image would resemble an outline that can be in Rhino. <p>
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/pexels-anna-shvets-4587992_backgroundremoved_corgi.png" height=250px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/pexels-prasanth-inturi-1051838-backgroundremoved_outline.png" height=250px> 
<img src="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Dancing_BackgroundRemoved.png" height=250px>

## Step 3: Rhino Model
I created a Rhino Model by smoothing out the lines, creating an offset of the trace, cleaning up the image and then I used the extrude curve in order to get the height to ~1 inch for each cookie cutter.
<p>
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Corgi.stl"> STL Corgi Link</a></p>
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Dancer.stl"> STL Dancer Link</a></p>
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Namaste.stl"> STL Namaste Yoga Link</a></p>

## Step 4: Rhino Files (for Reference)
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Corgi.3dm"> Corgi Rhino</a></p>
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/Dancer.3dm"> Dancer Link</a></p>
<a href="https://github.com/autarky-hash/autarky-hash.github.io/blob/main/NamasteCookieCutter.3dm"> Namaste Yoga Link</a></p>

