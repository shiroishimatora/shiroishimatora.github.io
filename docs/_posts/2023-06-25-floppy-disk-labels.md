---
layout: post
title:  "Making reproduction floppy disk labels"
---
# WORK IN PROGRESS
# INTRO AREA

## Making a label template
The first step was to measure the front, spine, and rear label areas of a 3.5" floppy disk. The front label area is 2.75 inches wide and 2.125 (2 1/8) inches tall. The spine is 2.75 inches wide and 0.125 (1/8) inches tall. The rear label area is 2.75 inches wide and 0.5 inches tall. The three label areas sum together to form a 2.75 inch square with rounded corners. This makes a single label that wraps from the front to the rear.

![Label printable area sizes][image-1]

The next step was to create a new project in Pixelmator Classic. I made a canvas that's 2.75 inches wide and 2.75 inches high at 600 pixels per inch. I then locked the background layer to avoid accidentally dragging the background around the canvas and created a square shape on the canvas. I resized the square shape to 1650 (2.75") pixels wide and 1275 pixels (2.125") high to form the front label area. I gave it a light gray fill color to tell it apart from the background and set the border stroke to none so that it became borderless. I then added another square and resized it to 1650 pixels (2.75") wide and 75 pixels (0.125") high for the spine area and gave it a slightly darker gray fill. And a final square shape resized to 1650 pixels (2.75") wide and 300 pixels (0.5") high with a dark gray fill for the rear area. This makes a good template for a floppy disk label with clearly defined printable areas.


![Template][image-2]

## Making a Macintosh System Disk label
Now that I have a template, I can start creating reproduction floppy disk labels. The first label I made was for a Macintosh System Disk, the kind that uses the Picasso-style Mac logo. I found a few eBay listings for disks in this style and used them as a reference. The first step was to change the spine and rear fill color to red. I then added the copyright text and part number text in white Helvetica and placed them in rough approximation to how they appear on the original label. Text in the spine and rear areas must be rotated 180 degrees so that it appears correctly when the label is printed and applied to the disk. Early Mac disks did have text in the spine area, but I can't find a clear reference picture, so I left it out.

I can't accurately describe how I made the Macintosh title and SYSTEM DISK subtitle as I can't quite remember what I did to make them. To start, the font is Apple Garamond. For the Macintosh title, I did have to play with kerning until the spacing between letters looked correct. I then had to convert the text to shapes and vertically stretch it until it looked correct. And then add the little TM text box to the right of the title and played around with the spacing until it also looked correct. Much of the same applies to the SYSTEM DISK subtitle, it has a lot of kerning adjustments between letters and is stretched horizontally to look correct (most noticeable with the "D" in "DISK"). I then added a dotted line and changed the size of the dots and relative positions of the text and line until it looked correct. I found a monochrome red Apple logo and dropped it on the canvas, resizing and moving until the positioning appeared correct.

[image-1]:	/assets/images/floppy-disk-labels/label-area-size.jpeg
[image-2]:	/assets/images/floppy-disk-labels/template.jpeg