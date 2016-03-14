+++
author = "author"
date = "2016-03-14T07:06:27Z"
description = "I have been working with the site preview. There was a case of a very sticky cache and this doesn’t work well if you immediately would want to check changes. Site preview has also been moved to its own subdomain: preview.appernetic.io, and now it is also possible to view the site preview if you are not signed in, so it is easier to share the URL and collaborate."
draft = false
keywords = ["Site preview", "theme", ".gitignore" ]
tags = ["Apperentic Static Site Generator", "two", "Appernetic Service", "Git"]
title = "Minor enhancements and fixes"
topics = ["topic 1"]
type = "post"

+++
![Appernetic Service site preview enhancements][1]

## Site preview fixes and enhancements
There was a case of a very sticky cache and this doesn't work well if you immediately would want to check changes. Site preview  has also been moved to its own subdomain: **preview.appernetic.io**,  and now it is also possible to view the site preview if you are not signed in, so it is easier to share the URL and collaborate.

## Add a .gitignore to your theme repo
The bug we reported last week wasn't a bug. When you delete a theme, we have git delete everything, and it doesn't delete dot files. The fix is to add a **.gitignore** file to your theme repo and exclude files such as **.DS_Store**. 

This is how it can be done:

```
public/
.sass-cache/
.DS_Store
```

That's all for now, happy static blogging :)

  [1]: https://res.cloudinary.com/appernetic/v1457939591/c25ymnmuqsfsmqjkk52b
