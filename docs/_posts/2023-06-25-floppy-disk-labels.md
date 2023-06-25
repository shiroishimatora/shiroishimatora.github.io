---
layout: post
title:  "Making reproduction floppy disk labels"
---
# WORK IN PROGRESS
# INTRO AREA

# Making a label template
The first step was to measure the front, spine, and rear label areas of a 3.5" floppy disk. The front label area is 2.75 inches wide and 2.125 (2 1/8) inches tall. The spine is 2.75 inches wide and 0.125 (1/8) inches tall. The rear label area is 2.75 inches wide and 0.5 inches tall. The three label areas sum together to form a 2.75 inch square with rounded corners. This makes a label that wraps from the front to the rear.

![Label printable area sizes][image-1]

The next step was to create a new project in Pixelmator Classic. I made a canvas that's 2.75 inches wide and 2.75 inches high at 600 pixels per inch. I then locked the background layer to avoid accidentally dragging the background around the canvas and created a square shape on the canvas. I resized the square shape to 1650 (2.75") pixels wide and 1275 pixels (2.125") high to form the front label area. I gave it a light gray fill color to tell it apart from the background and set the border stroke to none so that it became borderless. I then added another square and resized it to 1650 pixels (2.75") wide and 75 pixels (0.125") high for the spine area and gave it a slightly darker gray fill. And a final square shape resized to 1650 pixels (2.75") wide and 300 pixels (0.5") high with a dark gray fill for the rear area. This makes a good template for a floppy disk label with clearly defined areas

![Template][image-2]

[image-1]:	/assets/images/floppy-disk-labels/label-area-size.jpeg
[image-2]:	/assets/images/floppy-disk-labels/template.jpeg