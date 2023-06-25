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

## The first era: Picasso logo
![System 1 label][image-3]

Apple used this style of label for disks that came bundled with Macintosh 128K and 512K. As far as I can tell, this style was used through System 2.0 in 1985. 

Now that I have a template, I can start creating reproduction floppy disk labels. The first label I made was for a Macintosh System Disk, the kind that uses the Picasso-style Mac logo. I found a few eBay listings for disks in this style and used them as a reference. The first step was to change the spine and rear fill color to red. I then added the copyright text and part number text in white Helvetica and placed them in rough approximation to how they appear on the original label. Text in the spine and rear areas must be rotated 180 degrees so that it appears correctly when the label is printed and applied to the disk. Early Mac disks did have text in the spine area, but I can't find a clear reference picture, so I left it out.

For the text on the front, I did have to play around with the kerning until the spacing between letters closely matched the reference photo. I then had to convert the title text to shapes and vertically stretch it until it looked correct. And then add the little TM text box to the right of the title and played around with the position until it also appeared to match the reference photo. Much of the same applies to the SYSTEM DISK subtitle, it has a lot of kerning adjustments between letters and is stretched horizontally to look correct (most noticeable with the "D" in "DISK"). I then added a dotted line and changed the size of the dots and relative positions of the text and line until it visually matched the reference photo. I found a monochrome red Apple logo and dropped it on the canvas, resizing and moving until the positioning appeared correct.

The last two elements are the Picasso-style Macintosh logo and its trademark. This was probably the easiest part, I found a fairly clean copy of the logo and used the eraser tool to remove the white background. I then placed it on the canvas and resized it so that it looks approximately the correct size and position. I then ensured the logo aligned with the left edge of the title and subtitle text and that the spacing between the subtitle and top of the logo looked correct. That's about it for this style of label.


**This next label is one I'm quite proud of: MacWrite • MacPaint disk**

![MacWrite • MacPaint][image-4]

I found an eBay listing for the disk and used that picture as a baseline. I made a new canvas, dropped in the image, and stretched the image to 200% and began tracing over it. After about an hour of manually retracing it, I made a discovery: the paint bucket tool in Pixelmator is smart! Similar to how the eraser tool can be used to select areas of similar color to be removed, the paint bucket can select areas of similar color to be painted over without affecting other lines nearby or the background. This dramatically simplified the process as I just had to use the paint bucket to paint over the lines and smooth out the edges. I chose a mustard-like yellow for the MacPaint portion and ketchup-like red for the MacWrite portion of the drawing. It turned out rather well.

## The second era: FatBits icons
![MacDraw][image-5]

Apple used this style of label starting in 1984 for Macintosh applications that did not come bundled with the system. This style was also used for Lisa Office System 3.0 disks and disks that came bundled with Macintosh Plus and Macintosh 512Ke. These label designs are a lot simpler as they have just a FatBits bitmap of the app icon and a rainbow Apple logo. The early version of this design is notable for having the platform name in large type on the rear ("Macintosh" or "Lisa 7/7"), this aspect was dropped sometime in 1985.

[image-1]:	/assets/images/floppy-disk-labels/label-area-size.jpeg
[image-2]:	/assets/images/floppy-disk-labels/template.jpeg
[image-3]:	/assets/images/floppy-disk-labels/system-1.jpeg
[image-4]:	/assets/images/floppy-disk-labels/mw-mp.jpeg
[image-5]:	/assets/images/floppy-disk-labels/macdraw.jpeg