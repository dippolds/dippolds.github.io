---
id: 94
title: 'Migrating from Godaddy to Hostgator for WordPress blogs'
date: '2013-10-02T21:01:08-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=94'
permalink: /2013/10/02/migrating-from-godaddy-to-hostgator-for-wordpress-blogs/
categories:
    - Tech
format: false
---

## Objective

 Move 3 Wordpress blogs from Godaddy to Hostgator due to Godaddy slowness and business practices. Keep Hover.com as DNS registrar. ## Method

1. Order baby hosting service from Hostgator 1 week before Godaddy host service ends.
2. Disable "automatic renewal" on Godaddy account.
3. Go into each blog in Wordpress and Export the site to a local file on your computer, just in case.
4. Once Hostgator account is in place, request migration by supplying Hostgator with your Godaddy credentials.
5. Agree to pay ~$40 extra for 2 Wordpress migrations as only 1 is free
6. Hostgator will provide notice that the copy is complete and to test that it is working.
7. To test requires fooling your computer to go the new site by adding temporary entries into a local hosts file. In other words, fool your computer to go to a different site.
8. Once satisfied that everything is working, log in to Hover and point the DNS entries to the 1 IP address provided by Hostgator. Remove the host file entry and wait &lt;1 day. This can be a little confusing but to be clear, all the DNS entries point to the same IP address. The routing to the right site happens due to the next step.
9. On the Hostgator cPanel, use Add-on domains function to point the different DNS names to the right folder for the respective Wordpress blog. If you want another DNS entry to point to the same blog, add another entry for that one with the same path.
10. Hostgator and Hover provide excellent phone and email support if trouble occurs.
 