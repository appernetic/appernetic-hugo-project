+++
author = "author"
date = "2016-04-09T05:53:13Z"
description = "description"
draft = true
keywords = ["key", "words"]
tags = ["one", "two"]
title = "how to set up a static hugo website on github pages"
topics = ["topic 1"]
type = "post"

+++
A static website is fast and secure but it is not easy to start a new blog or website if you don't know a lot of commands, tools and also how to install them.

 1. List item
 2.  You have to download the right version of the static site generator for your OS and architecture.
 3.  You have to Install git
 4.  You have to create a GitHub, Bitbucket, Dropbox or Amazon S3 account or set-up a web server with a web Host.

Then when the installation and configuration are ready there are lots of steps to just have the website up and running on the Interwebz.

Before I created Appernetic.io I had to do all these 17 steps in terminal :

 
  hugo new site blog 
  cd blog
   hugo new post/easy-peasy.MD
 ```
   
Open the file and create content.

 ```
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
```

You have just published your first blog! Check your live server at: http://easypeasy.github.io

This steps will take at least 30 min if you have the knowledge. Now we do the same with Appernetic.io,

We assume the following is already done:
1. You have signed up for a subscription.
2. You have created a GitHub account.

Watch the instructive video for 2:13 minutes.
.
