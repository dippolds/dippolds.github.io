---
id: 60
title: 'Using Video from the Samsung Sports Camera'
date: '2006-07-15T15:52:00-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=60'
permalink: /2006/07/15/using-video-from-the-samsung-sports-camera/
blogger_blog:
    - blog.seandippold.com
blogger_permalink:
    - /2006/07/using-video-from-samsung-sports-camera.html
transfer_image:
    - 'yes'
categories:
    - Tech
format: false
---

The Samsung Sports Camera is a handy solid-state camcorder that produces MPeg4 video that does not work well with many video editors. The camera produces DIVX/XVid MPeg4 with a different fourCC signature (SEDG) forcing most software to use Samsung's own video decoder (CODEC). While playback with Windows Media player works well if you have Samsungs codec, use of tools to edit and covert the video reveal a variety of problems.

- Windows Movie Maker 2.1 - prone to crash
- Adobe Premier Elements 1.0 - does not accept clips
- Adobe Premier Elements 2.0 - accepts and previews clips but audio is dropped when rendering to a different format (like DVD)
- VideoStudio 9.0 LE (included with camera) - rendered video is shaky
 
 Through trial and error (and no help from Samsung), the following somewhat tedious steps result in a quality rendering of the video from the camera. 1. Install the DIVX (tested) or the XVID (untested) codec
2. Copy the clips to somewhere so the originals are not lost
3. Use a file editor like UltraEdit to change "SEDG" fourCC codes of each file to "DX50" (for DIVX) or "XVID" (if you prefer the Xvid codec). I.e. Search all \*.avi files the string "SEDG" and replace it with string "DX50". There are utilities to do this for one file but none I found will work on multiple files. The camcorder creates a file every time the video is paused so there tend to be many files.
4. Import the files into Adobe Premier Elements. Add the clips to the timeline and use Premier normally.
5. For each clip (this is the tedius part), right click on the timeline and select<span> field options</span>. Check the <span>Reverse Field Order</span> checkbox.
6. Export to DVD (or whatever) and the results should be of reasonable quality.
 
 <span>Postscript 6/2007</span> After many years as a Windows user, Apple's switch to standard Intel hardware tipped the balance and made me take the Mac plunge. The Samsung Sports Camera is even less Mac friendly but the solution on the Mac was much easier to find. 1. Buy and install [VisualHub](http://www.techspansion.com/visualhub/seeit.php). At $23, it handles all conversion needs. 2. Not sure other codecs are needed. Since VisualHub offer a trial version, give it a try without the codecs. If it doesn't work, add the Samsung and DIVX codec. 3. Batch convert all files into DV before using in iMovie. Selecting Advanced - Deinterlace may help with high speed movement flicker &amp; <span> Forcing ffmpeg Decoding in the Advanced panel.</span>