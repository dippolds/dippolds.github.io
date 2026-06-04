---
id: 512
title: 'Mac file copy to FAT drives that ignores files greater than 4Gb'
date: '2013-11-30T11:17:51-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=512'
permalink: /2013/11/30/mac-file-copy-to-fat-drives-that-ignores-files-greater-than-4gb/
categories:
    - Tech
format: false
---

FAT formatted drives cannot handle files &gt;4G in size. The below command copies all files preserving the directory structure but skips the files &gt;4Gb on a Mac or Linux. 1. Open Terminal and use this command **rsync -av --max-size=4G-1 */path/to/source/\** */path/to/destination/*** a - means archiving (keep files as-is) v - mean verbose and lists the names as they copy -max-size=4G-1 - means only copy files &lt; 4Gb in size Windows users need to install rsync separately.