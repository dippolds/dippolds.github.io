---
id: 560
title: 'Multiple Airport Express wifi installation'
date: '2013-12-09T23:49:33-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=560'
permalink: /2013/12/09/multiple-airport-express-wifi-installation/
categories:
    - Tech
format: false
---

Our house has about 15 wifi devices between phones, computers, tablets, security cameras and TV's. The 2-foot stone walls and multiple stories require more than one wireless hotspot to get acceptable coverage throughout the house.

## Equipment

 Currently using relatively old Apple Airport Express and Timecapsule (1st generation). These devices do have the N protocol but have limited antenna flexibility. Apple hotspots are generally about 2-times the price of other devices but generally easier to configure and paying $100 rather than $50 may be worth less aggravation. Recommend if possible staying with the same manufacturer for all devices as configuration can be significantly different vendor to vendor. ## Placement

 Tried to keep each hotspot (HS in diagram) to 1 wall or floor distance from a device. [![PechinsPost Wifi Hotspot placement](/wp-content/uploads/2013/12/PechinsPost-Wifi-Hotspot-placement.png)](/wp-content/uploads/2013/12/PechinsPost-Wifi-Hotspot-placement.png)## Configuration

 Each hotspot is wired by ethernet. Each hotspot is configured to be [roaming](http://support.apple.com/kb/HT4260) except for the primary base station. Changed each hotspot to use one channel (1 or 6 or 11) so there is no conflict. The automatic setting set by default may work just as well. ## Interference

 While the above configuration provides a strong signal everywhere, radical network slow-downs happen occasionally. Interference caused by our geothermal heatpump is the main suspect as the most common interference sources have been eliminated. Typical culprets are - Cordless phones (use 900MHz versions to avoid problems)
- Microwaves
 
## More Details to troubleshoot signal issues

 OSX Mavericks has a nice Wifi diagnostic tool that can help troubleshoot issue but the utility is a little hard to find intuitively. 1. Hold Option key and click the wifi symbol in the upper right of the screen
2. Click Open Wireless Diagnostics (likely will be prompted for your Mac password)
3. Click Window, Utilities
4. Click **Wi-Fi Scan** to show all Wifi access points and their signal strength and recommended available channels.
5. Click **Performance** to show a continuous graph of signal to noise ratio (SNR). Note how it changes as devices like microwaves are used to isolate the troublesome interference.
 
 [![wifi performance](/wp-content/uploads/2013/12/wifi-performance.png)](/wp-content/uploads/2013/12/wifi-performance.png) In this time period, the SNR was between 35 and 42. The [reference provides](http://www.enterprisenetworkingplanet.com/netsp/article.php/3747656/WiFi-Define-Minimum-SNR-Values-for-Signal-Coverage.htm) a key to provide insight; - &gt; 40dB SNR = Excellent signal (5 bars); always associated; lightning fast.
- 25dB to 40dB SNR = Very good signal (3 - 4 bars); always associated; very fast.
- 15dB to 25dB SNR = Low signal (2 bars); always associated; usually fast.
- 10dB - 15dB SNR = Very low signal (1 bar); mostly associated; mostly slow.
- 5dB to 10dB SNR = No signal; not associated; no go.