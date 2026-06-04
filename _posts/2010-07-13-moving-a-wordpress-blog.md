---
id: 29
title: 'Moving a WordPress blog'
date: '2010-07-13T11:48:00-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=29'
permalink: /2010/07/13/moving-a-wordpress-blog/
blogger_blog:
    - blog.seandippold.com
blogger_permalink:
    - /2010/07/moving-wordpress-blog.html
transfer_image:
    - 'yes'
categories:
    - Tech
format: false
---

Problem Had trouble updating the underlying GoDaddy MySQL to version 5.0 required by Wordpress 3. Solution Create a new Wordpress site on same hosting server and migrate the data Steps 1. Export content to XML in Wordpress admin console 2. Create a new Wordpress blog (which also creates a new MySQL instance) 3. Import the XML content into the new Wordpress blog 4. If using a custom them, copy the contents of the theme folder in Wordpress to the new Wordpress site 5. On New Wordpress site admin console, change path to existing Wordpress URL 6. On Old Wordpress site admin console, change path to a name like blog\_old for the Wordpress URL 7. Via a FTP client, rename the production blog folder to blog\_old 8. Via a FTP client, rename the new blog directory to the production folder name