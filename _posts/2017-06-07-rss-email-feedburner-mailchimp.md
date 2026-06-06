---
id: 1132
title: 'RSS email from Feedburner to Mailchimp'
date: '2017-06-07T10:38:40-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=1132'
permalink: /2017/06/07/rss-email-feedburner-mailchimp/
categories:
    - Lazy
format: false
---

Google has a service called Feedburner that allows people to subscribe to getting an email when new posts appear on a blog. Google hasn't been improving the service and there are better services available, namely MailChimp and ConstantContact. [![](/assets/img/uploads/2017/06/feedburner.png)](/assets/img/uploads/2017/06/feedburner.png) For low volumes of subscribers and emails, MailChimp is free so it makes most sense for a small blog. The conversion steps are pretty straightforward;

1. Export your subscribers list from Feedburner (Publicize, About Subscribers, Export CSV).
2. Create a MailChimp account and create a list. Import the CSV file.
3. Create a Campaign and pick the type Blog to email.
4. Create an email template remembering to pick the RSS Header and RSS Body.
5. Go to the subscriber list and click Sign-up forms.
6. Take the HTML generated in Sign-up forms and replace the Feedburner form with this code on your website. In Wordpress, that is usually under Appearance, Widgets, and a Text box.
 
 <style type="text/css">
	#mc_embed_signup{background:#fff; clear:left; font:14px Helvetica,Arial,sans-serif; }<br /></style><div id="mc_embed_signup"><form action="//LivesArchived.us16.list-manage.com/subscribe/post?u=59cc986dc1e95e5262d704d7e&id=7b86a57a83" class="validate" id="mc-embedded-subscribe-form" method="post" name="mc-embedded-subscribe-form" novalidate="" target="_blank"><div id="mc_embed_signup_scroll">## Subscribe to receive new posts

<div class="mc-field-group"><label for="mce-EMAIL">Email Address </label> <input class="required email" id="mce-EMAIL" name="EMAIL" type="email" value=""></input></div><div class="clear" id="mce-responses"></div> <div style="position: absolute; left: -5000px;"><input name="b_59cc986dc1e95e5262d704d7e_7b86a57a83" tabindex="-1" type="text" value=""></input></div><div class="clear"><input class="button" id="mc-embedded-subscribe" name="subscribe" type="submit" value="Subscribe"></input></div> </div> </form></div> <script src="//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js" type="text/javascript"></script><script type="text/javascript">(function($) {window.fnames = new Array(); window.ftypes = new Array();fnames[0]='EMAIL';ftypes[0]='email';fnames[1]='FNAME';ftypes[1]='text';fnames[2]='LNAME';ftypes[2]='text';}(jQuery));var $mcj = jQuery.noConflict(true);</script> 