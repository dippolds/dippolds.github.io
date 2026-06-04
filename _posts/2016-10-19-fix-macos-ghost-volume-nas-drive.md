---
id: 985
title: 'Fix for MacOS ghost volume NAS drive'
date: '2016-10-19T12:12:31-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=985'
permalink: /2016/10/19/fix-macos-ghost-volume-nas-drive/
categories:
    - Tech
tags:
    - fix
    - MacOS
    - NAS
format: false
---

Newer versions of MacOS (OSX) have a irritating bug where mounted volumes disconnect in Finder. Sometimes, when Finder reconnects, it creates a 2nd mount with a new name like volume**-1** and the original volume path doesn't work. For applications like Crashplan that use the Unix mount volume in the path, the application fails to see the volume is mounted. To get rid of the "ghost" mount, do the following; Mount the volume in Finder (in my case, a QNAP NAS called \\\\qnap\\homes) Open Terminal <span class="s1">$ cd /Volumes </span><span class="s1">$ ls</span><span class="s1"> Macintosh HD homes homes-1 *this shows the ghost volume (homes) and the active volume (homes-1)*</span>

In Finder, Eject the volume *this will remove the volume-1 working volume* In Terminal <span class="s1">$ sudo rm -rf homes *this removes the ghost volume* </span><span class="s1">$ ls </span><span class="s1">Macintosh HD *shows no volumes mounted*</span>

In Finder, mount the network volume In Terminal <span class="s1">$ ls </span><span class="s1">Macintosh HD homes *shows the Finder mounted volume is correctly named*</span>

[A similar article for the same issue in USB hard drives.](http://superuser.com/questions/20879/how-to-remove-duplicate-ghost-network-drive-on-os-x)

Example screenshot showing volume path

![crashplan_backup_volume](/wp-content/uploads/2016/10/crashplan_backup_volume.jpg)