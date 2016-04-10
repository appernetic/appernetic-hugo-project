+++
author = "Göran Svensson"
date = "2016-04-09T05:53:13Z"
description = "A static website is fast and secure but it is not easy to start a new blog or website if you don’t know a lot of commands, tools and also how to install them."
draft = false
keywords = ["Hugo static website generator", "Interwebz", "Appernetic"]
tags = ["Static website generator", "Hugo", "How to"]
title = "How to set up a static hugo website on github pages in 2 minutes"
topics = ["topic 1"]
type = "post"

+++
![A static website - appernetic.io][1]

***A static website is fast and secure but it is not easy to set up a new blog or website if you don't know a lot of commands, tools and also how to install them when you would rather like to be writing exciting content to distribute over the intermingling webz!***
 
First you have to:

 - download the right version of the static site generator for your OS and architecture.
 -  install git
 - create a GitHub, Bitbucket, Dropbox or Amazon S3 account or set-up a web server with a web Host.

Then when the installation and configuration are ready there are lots of steps to just have the website up and running on the Interwebz.

Before I created Appernetic I had to do all these 17 steps in the terminal after installation and configuration :

 
    hugo new site blog 
    cd blog
    hugo new post/easy-peasy.MD
 
   
Then open the file in a text editor and  write content, then dive back in to terminal:

    mkdir themes 
    cd themes 
    git clone https://github.com/appernetic/hugo-bootstrap.git
    hugo undraft content/post/easy-peasy.md
    hugo --theme=hugo-bootstrap
    mkdir blog-public
    cd blog-public
    git init
    git remote add origin https://easypeasy:236102a7cf231y2a5084a4847e0de99e636e391c@github.com/easypeasy
    cp -r ../blog/public/ .
    git add --all
    git commit -am ”Publish site”
    git push origin master


You have just published your first blog! Check your live server at:

     http://easypeasy.github.io (do not click this is just an example)

All these 17 steps will take at least 30 min if you have the knowledge. Now we do the same with Appernetic.

We assume the following is already done:

 1. You have signed up for a subscription.
 2. You have created a GitHub account.

**Now watch this instructive how-to video for 2:13 minutes.**

{{< vimeo 162159974 >}}

What about custom domains?
==========================

  
No problem, it is easy to connect your custom domain to your GitHub Pages. 

Place this file in your appernetic-hugo-project repositorys static folder:

Filename: CNAME

    blog.easypeasy.com

Here you can see how [we did this][2].

That's it! Give fast, secure blogging a try and you will never go back to WordPress, Joomla or Drupal. We support you both in Swedish and English.

  [1]: https://res.cloudinary.com/appernetic/v1460186011/k1seurwnwzitp8tbchvx
  [2]: https://github.com/appernetic/appernetic-hugo-project-1/blob/master/static/CNAME
