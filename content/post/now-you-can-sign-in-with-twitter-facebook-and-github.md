+++
author = "Göran Svensson"
date = "2016-04-26T13:10:05Z"
description = "Update! After users having expressed concerns about privacy we contemplated the implications over the weekend what impact it would have to add a custom sign up and log in with e-mail and a user-generated password."
draft = false
keywords = ["E-mail sign up", "Twitter", "Facebook", "Sign in", "Auth0"]
tags = ["Appernetic Static Site Generator", "Appernetic Service", "Enhancements"]
title = "Now you can sign in with twitter, facebook, github or your e-mail!"
topics = ["Enhancements"]
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


Sign in with your E-mail, Twitter, Facebook and GitHub.  Enjoy folks!

UPDATE (28052016): I have just removed Twitter user sign-in. It was an easy decision. Twitter users had no email in their meta info and was lagging behind in the interwebs, and behaved inconsistently. Also, I had no Twitter freemium or paying users and I had exceeded Auth0’s social connection limits anyway.

https://appernetic.io #contentmanagement


  [1]: https://res.cloudinary.com/appernetic/v1461667876/bvzstocens1wcwu3vba1
