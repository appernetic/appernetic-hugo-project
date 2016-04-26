+++
author = "Göran Svensson"
date = "2016-04-06T04:34:49Z"
description = "Now you can sign in with Twitter, Facebook and GitHub"
draft = false
keywords = ["E-mail si", "Twitter", "Facebook", "Sign in"]
tags = ["Appernetic Static Site Generator", "Appernetic Service", "Enhancements"]
title = "Now you can sign in with twitter facebook and github"
topics = ["topic 1"]
type = "post"

+++
## Update!

After users having expressed concerns about privacy we contemplated the implications over the weekend what impact it would have to add a custom sign up and log in with e-mail and a user-generated password.  

![Appernetic Static Site Generator with e-mail sign up, Twitter, Facebook and GitHub sign in!][1]

For us and the service there is the problem with:

* Users that are not verified signing up
* Maintaining a user database
* Users that are not following GitHub Pages policy
* Sending out verification e-mail to users
* Developing and testing

Everything has a cost. In the end, we decided to implement it with Auth0 and it was liberatingly simple to implement. No server side or client side development and the time-consuming testing and then gulp minifying and annotation. 

Just flip a switch in the auth0 dashboard.


We have just released a new version! Now you can sign in with your E-mail, Twitter, Facebook and GitHub.  Enjoy folks!

https://appernetic.io #contentmanagement


  [1]: https://res.cloudinary.com/appernetic/v1461667876/bvzstocens1wcwu3vba1
