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

1. You have to download the right version of the static site generator for your OS and architecture.
2. You have to Install git
3. You have to create a GitHub, Bitbucket, Dropbox or Amazon S3 account or set-up a web server with a web Host.

Before Appernetic.io:
We assume the following is already done:
1. You have downloaded the appropriate Hugo version for your OS and architecture.
2. Installed git
3. You have created a GitHub account
4. You have set up GitHub Pages

Then you have left to do this:
1. hugo new site blog 
2. cd blog
3. hugo new post/easy-peasy.md 
4. open file
5. edit file
6. mkdir themes 
7. cd themes 
8. git clone https://github.com/appernetic/hugo-bootstrap.git
9. hugo undraft content/post/easy-peasy.md
10. hugo --theme=hugo-bootstrap
11. mkdir blog-public
12. cd blog-public
13. git init
14. git remote add origin https://easypeasy:236102a7cf231y2a5084a4847e0de99e636e391c@github.com/easypeasy
15. cp -r ../blog/public/ .
16. git add --all
17. git commit -am ”Publish site”
18. git push origin master
17. You have just published your first blog! Check your live server at: http://easypeasy.github.io

Now we do the same with Appernetic.io,

We assume the following is already done:
1. You have signed up for a subscription.
2. You have created a GitHub account.
