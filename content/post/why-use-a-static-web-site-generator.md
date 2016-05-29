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
## Full circle with static websites
![Hugo plus octocat][1]
Today we have come full circle with static website generators. A long time ago at the end of 1994 I built a static website for the Swedish Tourist Association that contained hundreds of handcrafted html pages, it was quite advanced with a email to fax gateway that sent out bookings to remote mountain stations. Then I found ColdFusion in the beginning of 1995 and the sites I built had dynamic content served from MS Access databases. Later I started to use mySQL and built my own hosted CMS that was easily updated by non-technical users. 

## The programmable web
It was a lot of things to manage, servers, operating systems, security patches, databases, backup and on the application level with different versions and dependencies. Then I moved on to Platform as a Service (PaaS) and I only needed to manage and secure my applications, databases was now managed by a BaaS (backend as a service) and if I needed something specific such as commenting, search, email service or calendar there was always an API to connect to. The programmable web was born. 

## Advantage static website generators
Now there is a rich ecosystem of service providers for anything including forms, calendars, content, images, email, e-commerce etc. A dynamic CMS is no longer the best option for a website. There is really only a need for dynamic websites if you have a very large site with a complex structure and rich content such as news sites and large enterprises that have content that is updated very frequently. With a [static website][2] generator you didn’t really lose anything of practical value. Instead you have several advantages with a *static website* such as:

 - **Fast**, static files can be served fast. There is no database or templating layer that slows requests down. A static website will always be the fastest way to deliver content.
 - **Secure**, static websites do not contain dynamic content, and are therefore immune to most common attacks that dynamic systems like Wordpress and Joomla are plagued with.  Recently 12 million Drupal sites needed emergency patching.
 - **Previewable**, It is easy to separate preview from the live website.
 - **Versioning**, static website generators store their content in flat text files. This makes them ideal to be used with version control systems, such as Git. 

Static website generator are getting more popular and a view on Google Trends shows this:
 ![Static site generator statistics][3]

Interest over time. Web Search. Worldwide, 2004 to the present.

## A static website generator as a service
With Appernetic we are building a static website generator as a service that is easy to use for non-technical users and add some extra value. To start with we have included an easy to use editor, visual tree view, image upload, site preview, continuous integration with GitHub and atomic deploy, auto save and theme cloning. 

## Why gitHub?
You're probably wondering why the heck we are using GitHub. First of all GitHub use git which is a very good versioning system and they have [GitHub Pages][4] and you can use your own domain name and SSL (probably not the safest, but anyway its SSL!). Even if they only cache pages for 10 minutes and there are more cache misses then hits they have a fast CDN, Fastly.  I did a little unscientific performance test to see how it's really working out. All tests is done with [websitetest.com][5] from Berlin:

1. https://appernetic.io/#/about, with Cloudflare CDN and SSL, Dynamic site, 4.7 MB, Time to Last Byte: **70 ms**
2. https://appernetic.github.io/2016/02/10/firstpost/, with Fastly CDN and SSL, Static Blog Site 1.6 Mb, Time to Last Byte: **171 ms**
3. http://apple.com, No SSL, Dynamic site, 741 KB, Time to Last Byte: **378 ms**
4. http://www.theguardian.com/uk-news,  No SSL, Dynamic site, 4.3 MB, Time to Last Byte: **484 ms**
5. https://medium.com/@erinleecarr/lessons-dbbaa0c8294d#.h25nipmyq, SSL, Dynamic blog, 3.2 MB, Time to Last Byte **492 ms**.

> A static website wins every time even if there is a lot of cache misses.

We also eat our own dog food and use it for everything possible. Keep your eye on the blog where we will be posting tips and tricks how you can get the best advantage of a static blog or website.

![working on computer pexels.com][6]

We are using Hugo for fast website generation and GitHub for deploy. 


  [1]: https://res.cloudinary.com/appernetic/v1457306076/y8ylaazm8pet3nwpbffq
  [2]: https://appernetic.io
  [3]: https://res.cloudinary.com/appernetic/v1457306147/xm8rkllrfgr8xlznehix
  [4]: https://pages.github.com/
  [5]: http://websitetest.com/
  [6]: https://res.cloudinary.com/appernetic/v1457306218/e3v66ludnvfweghdb91d
