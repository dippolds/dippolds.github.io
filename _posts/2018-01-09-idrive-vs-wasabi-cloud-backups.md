---
id: 1224
title: 'iDrive vs. Wasabi for cloud backups'
date: '2018-01-09T11:47:13-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=1224'
permalink: /2018/01/09/idrive-vs-wasabi-cloud-backups/
evolve_sidebar_position:
    - default
evolve_full_width:
    - 'no'
evolve_hundredp_padding:
    - ''
evolve_page_title:
    - titlebar_breadcrumb
evolve_page_title_bar_bg_color:
    - ''
evolve_page_title_bar_bg:
    - ''
evolve_page_title_bar_bg_retina:
    - ''
evolve_page_title_bar_full_bg:
    - default
evolve_page_title_bar_parallax_bg:
    - default
evolve_widget_page:
    - 'no'
evolve_slider_position:
    - default
evolve_slider_type:
    - 'no'
evolve_revslider:
    - '0'
evolve_wooslider:
    - '0'
sbg_selected_sidebar:
    - 'a:1:{i:0;s:1:"0";}'
sbg_selected_sidebar_replacement:
    - 'a:1:{i:0;s:1:"0";}'
image: /wp-content/uploads/2018/01/cloudberry_backup_example-680x330.png
categories:
    - DIY
    - Tech
tags:
    - backup
format: false
---

People should not only backup their computers and phones but have at least one backup outside of their house to prevent loss from fire or theft. The best service was [Crashplan](https://www.crashplan.com) but they stopped their consumer service in 2017. Most of the technology press recommend [iDrive](https://www.idrive.com/) but after a year of using [iDrive](https://www.idrive.com/), the service and client software proved to be unreliable. While there are other turnkey solutions available, they are expensive (&gt;$100 a year for 2 people). After many trials and comparisons, [Wasabi](https://wasabi.com/) and [Cloudberry](https://www.cloudberrylab.com/) were selected. [Wasabi](https://wasabi.com/) is online cloud storage with the same interface as [Amazon's S3](https://aws.amazon.com/s3/). [Wasabi](https://wasabi.com/) has a simpler pricing model and lower prices than Amazon. 1 TB of storage costs $3.99 a month and they have a 1 month free trial. To store and retrieve, software for your computer is required. There is a lot to choose from but the key ones to consider are [Duplicacy](https://duplicacy.com/), [Duplicati](https://www.duplicati.com/), and [Cloudberry](https://www.cloudberrylab.com/). **Duplicacy**  *Pros* Efficient with storage *Cons* The user interface only supports backing up 1 folder. A future release should fix this $20 per user + $2/year ongoing **Duplicati** *Pros* Free *Cons* Requires installation of Microsoft Mono framework on Mac (lot of space and ? security) **Cloudberry - Winner** *Pros* Free for personal use on Mac Intuitive user interface *Cons* none [![](/wp-content/uploads/2018/01/cloudberry_backup_example.png)](/wp-content/uploads/2018/01/cloudberry_backup_example.png)

### Installation

1. Establish an account and set of keys on Wasabi. Follow the tutorial at \[embedyt\] https://www.youtube.com/watch?v=ABcIlXrhZZ4\[/embedyt\]
2. Install [Cloudberry Backup](https://www.cloudberrylab.com/backup/mac.aspx).
3. Run Cloudberry Backup, click Settings, and add Wasabi as a storage location. You will need to paste the access key and secret key setup in step 1.
4. Create a backup plan and select the folders you want backed up.
 
 If you have a NAS like QNAP, the NAS vendor likely has included backup software that can backup to Wasabi without the need for something like Cloudberry. The overall cost of this solution $48/year rather than $60/year for iDrive.