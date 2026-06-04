---
id: 782
title: 'Crashplan destination not found on Mac problem'
date: '2015-03-22T09:03:08-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=782'
permalink: /2015/03/22/crashplan-destination-not-found-on-mac-problem/
categories:
    - Lazy
format: false
---

Crashplan backs data to the cloud but also supports a local backup destination. Using a local destination allows a much quicker recovery (hours instead of days) because the local network is much faster than the internet.

### Issue

 Occasionally, Crashplan reports the Destination is not available even though the drive is shown connected in Finder. [![Screen Shot 2015-03-22 at 8.59.40 AM](/wp-content/uploads/2015/03/Screen-Shot-2015-03-22-at-8.59.40-AM-300x84.png)](/wp-content/uploads/2015/03/Screen-Shot-2015-03-22-at-8.59.40-AM.png)### Root Cause

 Mac OSX can generate phantom drives confusing Crashplan. ### Detection

 Open Terminal and execute this command *ls -laF /Volumes* drwxr-xr-x+ 3 userid admin 102 <span class="aBn" data-term="goog_309301410" tabindex="0"><span class="aQJ">Jan 15 20:40</span></span> 3\_TB\_WD/ drwx------ 1 userid staff 16384 <span class="aBn" data-term="goog_309301411" tabindex="0"><span class="aQJ">Oct 30 20:37</span></span> 3\_TB\_WD-1/ The duplicate drive with the -1 indicates that there is a phantom drive. If you were to disconnect the drive and run the command again, you will still see the drive. ### Corrective Actions

 1. Disconnect the network drive in Finder 2. Open Finder and using Go to go to \\Volumes 3. Delete the phantom drive 4. Reconnect to the real drive in Finder 5. Open Crashplan. Navigate to Backup, Destination. Click COMPACT. 6. At this point, Crashplan sees the drive and starts compacting and presumably when finished will back up [![Screen Shot 2015-03-22 at 9.00.06 AM](/wp-content/uploads/2015/03/Screen-Shot-2015-03-22-at-9.00.06-AM-300x166.png)](/wp-content/uploads/2015/03/Screen-Shot-2015-03-22-at-9.00.06-AM.png)### Preventative Measures

 There doesn't seem to be a way to automatically prevent this due to an underlying issue in OSX. Some users may not experience this depending on how they connect and i[f an application is writing when the drive is disconnected](http://superuser.com/questions/20879/how-to-remove-duplicate-ghost-network-drive-on-os-x). <div></div>