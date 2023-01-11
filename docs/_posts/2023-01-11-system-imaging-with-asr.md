---
layout: post
title:  "System Imaging with Apple Software Restore"
---
### The History of Apple Software Restore
Before it was rewritten as a command-line utility for Mac OS X, Apple Software Restore originated as a utility for System 7. Apple had commissioned Han Chen & Son Software Consulting Group to write ASR to assist Apple Authorized Service Providers in restoring customers’ Macs with a factory software image. It was first included in the **Apple Software Restoration CD - Market Software Series Volume 1.** This CD and other ones in the series contained system software restore “bundles” for Macintosh Performa and Macintosh LC computers. Another related CD, the **Apple Restoration CD, System Software Disk 1** is more relevant to my interests as it contains model-specific restore bundles for Macintoshes that shipped with System 7.0 and 7.1.

The first incarnation of Apple Software Restore was no more than a modified Apple Software Installer script. The second incarnation, version 1.1 included with the SSW Restoration CD, was a standalone application. Both perform the same function: erasing a user’s drive and restoring it to exactly how it was shipped from the factory.

Versions of ASR prior to 1.3 use Custom Mac Bundles rather than disk images. As ASR was a tool for use only by Apple and Apple-Authorized Service Providers, Apple did not document the format of custom Mac bundles or how to create them. The main structure is a folder with one subfolder and two documents. The name of the enclosing folder is the name of the bundle. The first document is a database of what appears to be a checksums of files in the bundle. It is named _(imagename).Database_. The second file is a text file describing the bundle, this is displayed to the user when the bundle is selected in ASR. It is named _(imagename).ReadMe_. The subfolder is the main content of the bundle, any file contained within is copied to the destination. It is named _(imagename)·(checksum)·_.

![The contents of a Custom Mac Bundle][image-1]

_The contents of a Custom Mac Bundle_

Optionally, there can be another subfolder called Bundle Actions and within it a folder called Post. An application in the Post folder will be run after the restore is complete. The only example I could find was a small application that renamed the destination volume to “Server HD” after the restore completed for a Workgroup Server software bundle.

ASR 1.3 and later use specially-prepared Disk Copy images instead of restore bundles. Restore bundles could still be used, but were deprecated. Further, unlike custom Mac bundles, the creation of disk images for ASR was documented. In 1998 with the release of ASR 1.3, Apple began shipping ASR to users on the Mac OS restore CDs bundled with each new Mac. The user would boot to the CD, launch ASR, select the image, and restore it to their drive.

![ASR as it was presented to the user on a software restore CD.][image-2]

_ASR as it was presented to the user on a software restore CD._

![ASR showing the disk image to be restored.][image-3]

_ASR showing the disk image to be restored._

Apple used ASR in their factories to deploy the shipping software image to the drive of each Mac that came off the assembly line. Apple continued development and use of ASR for manufacturing, end-user restore CDs, and IT/Computer Lab use into the early Mac OS X era. In fact, because ASR was not yet rewritten for Mac OS X, Apple’s restore CDs continued to boot to Mac OS 9 in order to use ASR to restore images of Mac OS X. This was used until the release of Mac OS X version 10.2 Jaguar, which had a Mac OS X-native version of ASR.

[image-1]:	/assets/images/system-imaging-with-asr/restore-bundle.png
[image-2]:	/assets/images/system-imaging-with-asr/asr-1.3-folder.png
[image-3]:	/assets/images/system-imaging-with-asr/asr-1.3.png