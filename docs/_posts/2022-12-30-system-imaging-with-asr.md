---
layout: post
title:  “System Imaging with Apple Software Restore”
---
Before being rewritten as a command-line utility for Mac OS X, Apple Software Restore originated as a utility for System 7. Apple had commissioned Han Chen & Son Software Consulting Group to write ASR to assist Apple Authorized Service Providers in restoring customers’ Macs with a factory software image. It was first included in the **Apple Software Restoration CD - Market Software Series Volume 1.** This CD and other ones in the series contained system software restore “bundles” for Macintosh Performa and Macintosh LC computers. Another related CD, the **Apple Restoration CD, System Software Disk 1** is more relevant to my interests as it contains model-specific restore bundles for Macintoshes that shipped with System 7.0 and 7.1.

The first incarnation of Apple Software Restore was no more than a modified Apple Software Installer script. The second incarnation, version 1.1 included with the SSW Restoration CD, was a standalone application. Both perform the same function: erasing a user’s drive and restoring it to exactly how it was shipped from the factory.

Versions of ASR prior to 1.3 use restore bundles rather than disk images. As ASR was a tool for use only by Apple and Apple-Authorized Service Providers, Apple did not document the format of restore bundles or how to create them. The main structure is a folder with one subfolder and two documents. The name of the enclosing folder is the name of the restore bundle. The first document is a database of what appears to be a checksums of files in the bundle. It is named _(imagename).Database_. The second file is a text file describing the restore bundle, this is displayed to the user when the bundle is selected in ASR. It is named _(imagename).ReadMe_. The subfolder is the main content of the restore bundle, any file contained within is copied to the destination. It is named _(imagename)·(checksum)·_

![The contents of a restore bundle][image-1]



[image-1]:	/assets/images/system-imaging-with-asr/restore-bundle.png