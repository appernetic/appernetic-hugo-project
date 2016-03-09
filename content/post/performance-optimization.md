+++
author = "Göran Svensson"
date = "2016-03-08T19:03:58Z"
description = "We have made significant performance improvements of our service and have dug deep into everything on the client and server side. All images is now sent with Cloudinary's Akamai CDN."
draft = false
keywords = ["Performance", "Optimization", "CloudFlare", "Webpagetest", "Cache"]
tags = ["Internet", "Performance Optimization", "Appernetic Service"]
title = "Performance optimization"
topics = ["topic 1"]
type = "post"

+++
## Performance improvements
We have made significant performance improvements of our service and have dug deep into everything on the client and server side. All images is now sent with Cloudinary's Akamai CDN including the favicon, and every css, html and Javascript file is compressed and minified. 

## Speed Index
We use [webpagetest][1] for our performance tests. As a measure of how one experiences the web page speed we use [Speed Index][2]. The Speed Index is the average time at which visible parts of the page are displayed.  It is expressed in milliseconds and dependent on size of the view port. 

![Speed Index Reference Results][3]
We have now also separated the routes for the front page and the Angular app. The Angular app are now between the median to 10th percentile compared to the reference speed index, which is as good as it can get. Our front page which we want to be as quick as possible is now below the 10th percentile 6 of 8 times.

Angular app performance test from:

 - Dulles, VA Thinkpad T430: http://www.webpagetest.org/result/160308_C8_15P4/1/details/  First View, Speed Index: 1422

 - San Francisco, CA USA - Yottaa:  http://www.webpagetest.org/result/160308_YB_15ZA/  First View, Speed Index: 2881

 - Singapore - EC2: http://www.webpagetest.org/result/160308_EC_166Y/  First View, Speed Index: 2884

 - Brussels, BE: http://www.webpagetest.org/result/160308_NP_162K/ First View, Speed Index: 2408

 - Frankfurt, DE: http://www.webpagetest.org/result/160308_RX_6P2/  First View, Speed Index: 3759

Front page performance test from:
 - Amsterdam: http://www.webpagetest.org/result/160309_E3_6HP/ First view, Speed Index: 600
 - Singapore: http://www.webpagetest.org/result/160309_DG_6HB/ First view, Speed Index: 769
 - Sydney, Australia (Servers Australia) http://www.webpagetest.org/result/160309_04_6GN/ First view, Speed Index: 1600
 - Johannesburg, South Africa http://www.webpagetest.org/result/160309_MC_6GQ/ First view, Speed Index: 1305
 - Seoul, Korea EC2 http://www.webpagetest.org/result/160309_85_6GZ/ First view, Speed Index: 1519
 - San Francisco, CA USA - Yottaa: http://www.webpagetest.org/result/160309_1S_83M/ First view, Speed Index: 1672
 - Dulles, VA - Thinkpad T430: http://www.webpagetest.org/result/160309_PX_87N/  First view, Speed Index: 900
 - Frankfurt, DE: http://www.webpagetest.org/result/160309_GG_8DS/ First view, Speed Index: 1309

Our uptime monitoring with Pingdom also shows that the we are on the [right track now][4]. For the front page we now have performance grade 92/100. Google PageSpeed Insights  

![Response time diagram last 24 hours][7]
Response time diagram last 24 hours.

![Pingdom test result logs for Appernetic service][6]
Pingdom test result logs.

## Caching
Caching with CloudFlare is improving. Once the cache has been properly warmed up, it will even be better than this.

![Appernetic service, caching with CloudFlare][5]
Appernetic service, caching with CloudFlare.


  [1]: http://www.webpagetest.org
  [2]: https://sites.google.com/a/webpagetest.org/docs/using-webpagetest/metrics/speed-index
  [3]: https://res.cloudinary.com/appernetic/v1457463274/gcgzrecgedcjnc3gzdj3
  [4]: http://stats.pingdom.com/r7vt9tv6brq8/2014082
  [5]: https://res.cloudinary.com/appernetic/v1457461947/hzs05zxjzr8otv2nrvka
  [6]: https://res.cloudinary.com/appernetic/v1457463057/rbouqv8jnwpfsadjssgk
  [7]: https://res.cloudinary.com/appernetic/v1457462773/atscsb7z2qtr4cn8qid0
