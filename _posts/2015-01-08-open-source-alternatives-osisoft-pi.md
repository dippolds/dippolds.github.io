---
id: 769
title: 'Open Source alternatives to OSISoft PI'
date: '2015-01-08T11:40:39-05:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=769'
permalink: /2015/01/08/open-source-alternatives-osisoft-pi/
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
    - Tech
format: false
---

OSISoft PI is the industry leader for [operational historians](http://en.wikipedia.org/wiki/Operational_historian%20). Historians take simple time-based data and store it for retrieval later. For example, a temperature probe sends the historian the value 10.1 degrees C at 2015-01-15 09:32:03 for storage. The probe sends an updated value every minute. Later, someone interested in that data trend retrieves the values from the historian and graphs it. Most people familiar with computers initially view this as a simple task and are surprised to hear companies pay for software to store this data and that there are so few alternatives. There are some emerging Open Source tools that may evolve to a complete solution in the future. The current options are [Open Time Series Database ](http://opentsdb.net/) - built on-top of big-data tools like Hadoop [Nimbit](http://www.nimbits.com/index.jsp) - Web-services oriented to internet of things [Mango Automation](http://infiniteautomation.com) - Open source automation software that also includes a historian. The key drawbacks to these tools over commercial software includes; **Interface variety** - Drawing data from different kinds of system requires different interfaces. The Open Source tools tend to support web service interfaces which is good if the sending system is customizable. **Request modes and interpolation** - Consider if for a particular data stream, a data point is stored every minute. When reading the stored the data, one may need a representation of the data for every hour or maybe to compare to another point at a certain second. For an end-user, this inconstancy adds a lot of work to the simply idea of showing a trend/graph of the data. **Large volume of data** - Imaging thousands of sensors sending data every second or more and the system simply recording it. Most commercial historians only store the data to the right time precision as by the requirements for that sensor. While placing an algorithm saves on space, the data is harder to use as the data must be uncompressed before it is readable.

## Open Source Operational Historians have a future

 Trends in technology are heading in the right direction to allow many more uses for open source operational historian over commercial software. Storage space costs are dropping rapidly reducing the necessity to to use compression. Analytic tools are improving to help with comparative data analysis. Interface technologies are moving away from Windows OLE and proprietary interfaces to web technology standards like [OPC UA](http://en.wikipedia.org/wiki/OPC_Unified_Architecture). ## Update - November, 2017

 Two years after this article was written there still isn't a comprehensive open source alternative to OSI PI and it is unlikely any OSISoft customer will jump of the Open Source trend. ### Data Storage

 A [recent review of the top time series databases](https://blog.outlyer.com/top10-open-source-time-series-databases) suggest there is no clear winner even on the database side of the solution. Many of these solutions are being driven by system/application monitoring rather than by sensor integration. ### Data collection and interfacing

 Internet-of-Things (IoT) rather than automation companies drives a lot of the modern open-source interfacing standards. [OPC-UA is available in many more places and has rich support](https://twitter.com/hashtag/OPCUA?src=hash) for different languages like NodeJS. ### Visualization and Analysis

 There continue to be an almost overwhelming number of open-source visualization tools but many don't cater to time-series databases. The selection of a tool will depend on which database is used. For example, [Prometheus database](https://prometheus.io/) works well with [Grafana](https://grafana.com/). Prometheus easily connects to most raw programming languages (like [Python](https://github.com/prometheus/client_python)) but tends not to be used with higher level analytical tools like MatLab.