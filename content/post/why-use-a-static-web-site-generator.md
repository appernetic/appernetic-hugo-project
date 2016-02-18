+++
author = "Admin"
date = "2016-02-10T19:50:09Z"
description = "With Appernetic we are building a static web generator as a service that is easy to use for non-technical users and add some extra value. To start with we have included an easy to use editor, visual tree view, image upload, site preview, continuous integration with GitHub, auto save and theme cloning."
draft = false
keywords = ["Static web site generator", "dynamic CMS", "Appernetic", "Fast", "Secure"]
tags = ["Static web site generator", "Internet"]
title = "Why use a static web site generator?"
topics = ["Static web site generator"]
type = "post"

+++
## Full circle
![Hugo plus octocat][1]
Today we have come full circle with static site generators. A long time ago at the end of 1994 I built a static web site for the Swedish Tourist Association that contained hundreds of handcrafted html pages, it was quite advanced with a email to fax gateway that sent out bookings to remote mountain stations. Then I found ColdFusion in the beginning of 1995 and the the sites I built had dynamic content served from MS Access databases. Later I started to use mySQL and built my own hosted CMS that was easily updated by non-technical users. 

## The programmable web
It was a lot of things to manage, servers, operating systems, security patches, databases, backup and on the application level with different versions and dependencies. Then I moved on to Platform as a Service (PaaS) and I only needed to manage and secure my applications, databases was now managed by a BaaS (backend as a service) and if I needed something specific such as commenting, search, email service or calendar there was always an API to connect to. The programmable web was born. 

## Advantage static web site generators
Now there is a rich ecosystem of service providers for anything including forms, calendars, content, images, email, e-commerce etc. A dynamic CMS is no longer the best option for a web site. There is really only a need for dynamic web sites if you have a very large site with a complex structure and rich content such as news sites and large enterprises that have content that is updated very frequently. With a static site generator you didn’t really lose anything of practical value. Instead you have several advantages with a static site such as:

 - **Fast**, static files can be served fast. There is no database or templating layer that slows requests down. A static site will always be the fastest way to deliver content.
 - **Secure**, static sites do not contain dynamic content, and are therefore immune to most common attacks that dynamic systems like Wordpress and Joomla are plagued with.  Recently 12 million Drupal sites needed emergency patching.
 - **Previewable**, It is easy to separate preview from the live site.
 - **Versioning**, static-site generators store their content in flat text files. This makes them ideal to be used with version control systems, such as Git. 

Static site generator are getting more popular and a view on Google Trends shows this:
 ![enter image description here][2]

Interest over time. Web Search. Worldwide, 2004 to the present.

## A static site generator as a service
With Appernetic we are building a static web generator as a service that is easy to use for non-technical users and add some extra value. To start with we have included an easy to use editor, visual tree view, image upload, site preview, continuous integration with GitHub and atomic deploy, auto save and theme cloning. 

## Why gitHub?
You're probably wondering why the heck we are using GitHub. First of all GitHub use git which is a very good versioning system and they have [GitHub Pages][3] and you can use your own domain name and SSL (probably not the safest, but anyway its SSL!). Even if they only cache pages for 10 minutes and there are more cache misses then hits they have a fast CDN, Fastly.  I did a little unscientific performance test to see how it's really working out:

1. https://appernetic.io/#/about, with Cloudflare CDN and SSL, Dynamic site, 4.7 MB, Time to Last Byte: **70 ms**
2. https://appernetic.github.io/2016/02/10/firstpost/, with Fastly CDN and SSL, Static Blog Site 1.6 Mb, Time to Last Byte: **171 ms**
3. http://apple.com, No SSL, Dynamic site, 741 KB, Time to Last Byte: **378 ms**
4. http://www.theguardian.com/uk-news,  No SSL, Dynamic site, 4.3 MB, Time to Last Byte: **484 ms**
5. https://medium.com/@erinleecarr/lessons-dbbaa0c8294d#.h25nipmyq, SSL, Dynamic blog, 3.2 MB, Time to Last Byte **492 ms**.

> A static site wins every time even if there is a lot of cache misses.

We also eat our own dog food and use it for everything possible. Keep your eye on the blog we will be posting tips and tricks how you can get the best advantage of a static blog or web site.

![working on computer pexels.com][4]

We are using Hugo for fast site generation and GitHub for deploy. 


  [1]: /images/hugo-octocat.png
  [2]: /images/statisgoole.png
  [3]: https://pages.github.com/
  [4]: /images/man-person-apple-iphone-opt.jpg
