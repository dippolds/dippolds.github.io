---
id: 1338
title: 'LastPass Replacement'
date: '2023-01-05T11:27:19-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'https://seandippold.com/?p=1338'
permalink: /2023/01/05/lastpass-replacement/
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
categories:
    - Lazy
format: false
---

LastPass recently announced [that customer password vaults were stolen over the summer](https://www.nytimes.com/2023/01/05/technology/personaltech/lastpass-breach-password-safety.html). As long as your master password was long and complex, it is unlikely any of your stored passwords could be cracked. [Based on a well-regarded security researcher Steve Gibson](https://twit.tv/shows/security-now/episodes/904), I switched to [BitWarden](https://bitwarden.com/) as a replacement. I elected the $10 a year account to allow more advanced multi-factor authentication and cloud vault storage.

## Key Points

- BitWarden is cheaper than Lastpass ($20/year for 2 accounts vs. $45)
- Same features but better encryption
- OpenSource version is both free and more transparent
- Migration is easy, export from LastPass, Import to Bitwarden. Removed LastPass apps and browser extension and add Bitwarden.
- Turned on Multi-factor authentication in Bitwarden and use the Google Authenticator app (and email as a backup)
- Backed up Google Authenticator to my iPad (that has a fingerprint lock)
- Recommend using Google Authenticator over SMS/Text in case you lose your number. Still, consider what your plan is if you lose your phone. You don't want to lock yourself out.
- The accounts that are critical like Google email &amp; bank accounts have their own MFA enabled so even if someone cracks my LastPass vault, what they have access to isn't valuable.
- People who only use Apple products should consider migrating their password manager to the free [Apple Keychain feature ](https://osxdaily.com/2022/07/22/import-passwords-icloud-keychain-mac/)

<figure class="wp-block-image size-large">![](https://raw.githubusercontent.com/bitwarden/brand/master/screenshots/web-vault-macbook.png)</figure>