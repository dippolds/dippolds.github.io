---
id: 78
title: 'Morocco GPS Waypoints'
date: '2005-05-24T21:15:00-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=78'
permalink: /2005/05/24/morocco-gps-waypoints/
blogger_blog:
    - blog.seandippold.com
blogger_permalink:
    - /2005/05/morocco-gps-waypoints.html
transfer_image:
    - 'yes'
categories:
    - Tech
    - Travel
format: false
---

Since the driving is largely unplanned, a GPS could be of assistance. A GPS isn't much help unless you have a paper map with LAT/LONG (most don't) or a computer with an integrated map of the area. We are not willing to tote a laptop and digital maps of Morocco are rare and expensive. So we are left with using the waypoint functionality built into the GPS. I thought it would be easy to get a list of Moroccian waypoints but I was wrong. I came up with this process to generate waypoints of most of the cities in Morocco. 1. Using [Microsoft Streets and Trips 2005](http://www.microsoft.com/streets/ProductDetails.aspx?pid=002), select cities in Morocco and choose Add Stop to Route. Save the map. MSS&amp;T had 200+ cities and towns in Morocco (but no roads). Accuracy is unknown but assumed to be acceptable. The product is only marketed for US &amp; Canada and only contains road in those countries. [Here is the MSS&amp;T .est file for Morocco with the stops. ](http://mywebpages.comcast.net/dippolds/200505_Morocco/waypoints_morocco.est) 2. Use freeware [st2gpx](http://gpsbabel.sourceforge.net/st2gpx/st2gpx.html) to get the MSS&amp;T .EST file in a more standard format (GPX). This is an XML file that can be editted with a text editor. For example, I removed the route section as it is of little use for an unplanned trip. [Here is the waypoint list for Morocco (GPX). ](http://mywebpages.comcast.net/dippolds/200505_Morocco/waypoints_morocco.gpx) 3. Use freeware [EasyGPS](http://www.easygps.com/) to send the waypoint data to the GPS. In my case, I have an Garmin eTrex that is probably about 3 years old. A paper map is still required and the best seems to be published by Michelin.