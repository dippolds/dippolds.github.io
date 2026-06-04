---
id: 1110
title: 'macOS Finder directory listing slow with QNAP NAS'
date: '2017-04-05T22:51:37-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=1110'
permalink: /2017/04/05/qnap-file-access-slow-mac-osx/
categories:
    - Tech
format: false
---

### Problem

 Accessing a QNAP network attached storage (NAS) file directory from macOS Finder could take 15-30 seconds. ### Solution

1. in Finder, Open the root level of share
2. click View, and uncheck Show Icon Preview. Then click **Use as Defaults**[![](/wp-content/uploads/2017/04/osx_show_icon_preview.png)](/wp-content/uploads/2017/04/osx_show_icon_preview.png)
 
### Rational

 macOS Sierra (and earlier versions) is checking each file and over a slower network link this can take a while if there are a number of files. In a case it went from 15 seconds to &lt; 1 second. [Credit](https://discussions.apple.com/thread/5500165?start=135&tstart=0)