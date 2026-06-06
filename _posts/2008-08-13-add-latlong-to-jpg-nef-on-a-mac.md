---
id: 41
title: 'Add Lat/Long to JPG and NEF on a MAC'
date: '2008-08-13T10:36:00-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=41'
permalink: /2008/08/13/add-latlong-to-jpg-nef-on-a-mac/
blogger_blog:
    - blog.seandippold.com
blogger_permalink:
    - /2008/08/add-latlong-to-jpg-nef-on-mac.html
transfer_image:
    - 'yes'
categories:
    - Tech
    - Travel
format: false
---

This technique uses Google maps to generate GPS coordinates and inserts the coordinates into JPG or raw photos. Requirements Mac [GPSPhotoLinker](http://oregonstate.edu/~earlyj/gpsphotolinker/index.php) - free [KLMtoGPX converter](http://www.fish-track.com/?page_id=3) - free Procedure 1. Create a new My Maps on Google maps with the places you visited (can also use Google Earth) 2. Export the points to a .klm file 3. Convert the .klm file using the program [KLMtoGPX converter](http://www.fish-track.com/?page_id=3) 4a. Manual (easy but requires you to select each photo) Run GPSPhotoLinker, Load GPX file, Load all photos, Select Manual tab, click each photo, select waypoint, click Save to photo 4b. For large number of photos - Use TextEdit to convert the Waypoint file into a Track file (both are XML) and set the time to be outside the time recorded in the photo (i.e. if the group of photos was taken between 9 and 10AM GMT, set the time on the two track points to be 8AM and 11AM). Click Batch convert and use the option Nearest Recorded Point. [![](/assets/img/uploads/2013/10/example+tracks.gpx_.jpg)](http://4.bp.blogspot.com/_XSvmZLvyQNw/SKNAvkZUOjI/AAAAAAAAAC0/li0i7UH_4D4/s1600-h/example+tracks.gpx.jpg)