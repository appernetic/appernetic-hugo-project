+++
author = "author"
date = "2016-03-08T18:21:10Z"
description = "description"
draft = true
keywords = ["key", "words"]
tags = ["one", "two"]
title = "Performance optimization"
topics = ["topic 1"]
type = "post"

+++


We use [webpagetest][1] for our performance tests. As a measure of how one experiences the web page speed we use [Speed Index][2]. The Speed Index is the average time at which visible parts of the page are displayed.  It is expressed in milliseconds and dependent on size of the view port. 

 - Dulles, VA Thinkpad T430: http://www.webpagetest.org/result/160308_C8_15P4/1/details/  First View, Speed Index: 1422
 - San Francisco, CA USA - Yottaa:  http://www.webpagetest.org/result/160308_YB_15ZA/  First View, Speed Index: 2881
 - Singapore - EC2: http://www.webpagetest.org/result/160308_EC_166Y/  First View, Speed Index: 2884
 - Brussels, BE: http://www.webpagetest.org/result/160308_NP_162K/ First View, Speed Index: 2408
 - Frankfurt, DE: http://www.webpagetest.org/result/160308_RX_6P2/  First View, Speed Index: 3759

Our uptime monitoring with Pingdom also shows that the we are on the right track now: http://stats.pingdom.com/r7vt9tv6brq8/2014082

Caching with CloudFlare is improving. 


  [1]: http://www.webpagetest.org
  [2]: https://sites.google.com/a/webpagetest.org/docs/using-webpagetest/metrics/speed-index