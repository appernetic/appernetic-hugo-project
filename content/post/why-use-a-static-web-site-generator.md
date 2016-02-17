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
![Hugo plus octocat][2]
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
<script type="text/javascript">
//function which gets screen width
function getWidth() {
  if (self.innerHeight) {
    return self.innerWidth;
  }
  if (document.documentElement \&& document.documentElement.clientHeight) {
    return document.documentElement.clientWidth;
  }
  if (document.body) {
    return document.body.clientWidth;
  }
}
  //define screen width variable. Subtract 15 pixels from width just to be on the safe side and reduce chance of getting a horizontal scroll bar
    var screenWidth = getWidth()-Number(15);
//replace the following URL with your own. Be sure to keep the modified part of the string in tact where it replaces the width with screenWidth variable
    var embedCode = "//www.google.com.au/trends/embed.js?hl=sv&q=static+site+generator&cmpt=q&tz=Etc/GMT-1&tz=Etc/GMT-1&content=1&cid=TIMESERIES_GRAPH_0&export=5&w="+screenWidth+"&h=330";
//write this new code to browser. Split '<script'> tags to prevent browser errors when writing.
document.write('<scr'+'ipt type=\"text/javascript\" src=\"'+embedCode+'\"></scr'+'ipt>');

</script>

Interest over time. Web Search. Worldwide, 2004 to the present.

## A static site generator as a service
With Appernetic we are building a static web generator as a service that is easy to use for non-technical users and add some extra value. To start with we have included an easy to use editor, visual tree view, image upload, site preview, continuous integration with GitHub and atomic deploy, auto save and theme cloning. We also eat our own dog food and use it for everything possible. Keep your eye on the blog we will be posting tips and tricks how you can get the best advantage of a static blog or web site.

![working on computer pexels.com][1]

We are using Hugo for fast site generation and GitHub for deploy. 


  [1]: /images/man-person-apple-iphone-opt.jpg
  [2]: /images/hugo-octocat.png
