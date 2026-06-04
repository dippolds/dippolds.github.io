---
id: 1036
title: 'Raspberry PI 3 with VGA monitor'
date: '2017-01-11T17:05:30-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=1036'
permalink: /2017/01/11/raspberry-pi-3-vga-monitor/
categories:
    - DIY
    - Tech
format: false
---

An old monitor can be turned into a pretty decent computer and gaming machine. It is a fun project to do with kids.

## Parts and Materials

1. [Raspberry PI Model 3 B](https://smile.amazon.com/Raspberry-Pi-896-8660-Model-Motherboard/dp/B01CD5VC92/) - $40
2. [Ableconn HDMI2VGAD Active HDMI to VGA Adapter Converter Dongle](https://smile.amazon.com/gp/product/B00JLRHMZE) - $15
3. [4GB to 32GB microSD card](https://smile.amazon.com/gp/product/B010Q57T02) - $5-$10
4. VGA monitor - usually free, preferably LCD to conserve electricity. Find out the resolution (like 1024 x 768) by searching the model number.
5. USB power adapter &amp; mini USB cable
6. USB keyboard and USB mouse
7. Glue gun, small screws, and small pieces of wood or plastic
8. Optional for gaming - SNES Retro USB Super Nintendo Controller For Windows PC/MAC - eBay $6
 
## Steps

1. Mount the Raspberry PI on the back of the monitor using risers, screws and a hot glue gun. See photo. There are cases available but this way makes the device accessible and low cost. \[caption id="attachment\_1043" align="alignnone" width="640"\]![Hot glue holding on PI to back of the monitor with wooden dowels](/wp-content/uploads/2017/01/pimount.jpg) Hot glue holding on PI to back of the monitor with wooden dowels\[/caption\]
2. On another computer, install a free program called [Etcher](https://etcher.io/). This software will allow you to install a Raspberry PI image on to the microUSB card.
3. Go to the Raspberry PI website and [download NOOBS (for new people) or Rasbian (a full-featured computer).](https://www.raspberrypi.org/downloads/) Use Etcher to install the image file onto the micoSD card.
4. Raspberry PI expects the monitor to be HDMI but in this case it will be USB. Edit a file on the microUSB called [config.txt](https://www.raspberrypi.org/documentation/configuration/config-txt.md). All of the settings are commented out using the # sign. 
    1. Remove the # from the line that says **hdmi\_safe**=1 to enable the safe mode
    2. We are going to edit this file again in the future but let's first see if everything works.
5. Plug everything together with the last thing being plugged in is the USB power supply. See the [PI Hardware Guide](https://www.raspberrypi.org/help/) for instructions and pictures. Note steps 2-4 are similar to the software guide but easier.
6. Power up and you should see a working computer in about a minute. \[caption id="attachment\_1045" align="alignright" width="209"\]![Raspberry PI running in low resolution](/wp-content/uploads/2017/01/pi_lowres.png) Raspberry PI running in low resolution\[/caption\] 7. It is likely the resolution is lower than the monitor supports (i.e. things are large). This step is a little more complicated and requires you to know the native resolution of your monitor. In this case, the resolution is 1024x768. You will need to review this document then pick the right settings for **hdmi\_group** and **hdmi\_mode** in the config.txt file. 
    1. Shut down the Raspberry PI and remove the microSD card and put it back in another computer.
    2. Remove the # signs from these two setting rows hdmi\_group and hdmi\_mode
    3. Change the numbers [per the table here](https://www.raspberrypi.org/documentation/configuration/config-txt.md) (see sections on hdmi\_group and hdmi\_mode)
    4. In this case, for a 1024x768 monitor the lines look like 
        1. **hdmi\_group=2**
        2. **hdmi\_mode=16**
    5. You also have to take it out of HDMI safe mode that was turned on in step 4 AND enable HDMI\_Force\_Hotplug resulting in lines that look like this 
        1. **\#hdmi\_safe=1**
        2. **hdmi\_force\_hotplug=1**
 
## Please Note

1. Most HDMI to VGA converters **do not work with Raspberry PI**. Use the one above or [make sure from this PI site it will work](http://elinux.org/RPi_VerifiedPeripherals#HDMI-.3EVGA_converter_boxes) and could break the Raspberry PI.
2. A cheap HDMI monitor may be as low as $60. Still more expensive than a $15 adapter but it is likely to be larger.
 
 \[caption id="attachment\_1044" align="aligncenter" width="300"\]![PI running full 1024x768 resolution](/wp-content/uploads/2017/01/pi_fullresolution-300x225.jpg) PI running full 1024x768 resolution\[/caption\]