+++
author = "author"
date = "2016-02-18T20:27:25Z"
description = "description"
draft = false
keywords = ["key", "words"]
tags = ["one", "two"]
title = "collaborating and working with hugo themes"
topics = ["topic 1"]
type = "post"

+++

Customizing themes
If you just have set up your Appernetic account you need to add a theme. The easiest way is to clone a theme which you can do from the drop down button beside the blue Preview button to the right. 

![enter image description here][1]

You probably want to customize the theme before you use it and have a theme that is matching your business web site or service. I am using Bootswatch Paper theme for [Appernetic service][2]. Fortunately I found [hugo-bootstrap][3] and cloned it. Then to customize it further I pressed the Sync button which does a pull and then a push to your Appernetic project repository at GitHub with the name appernetic.hugo-project . When you start out you will not have this repo so it is automatically created for you. 

![enter image description here][4]

Now to work with the theme I did a pull to my local computer, edited the theme with my favorite editor Atom and after that I did a commit and a push back to my GitHub project repo. If you are a hard-core git user you would start terminal and add the commands. There is also a very easy to use desktop client for GitHub.

![enter image description here][5]

Notice also that I have all the social and collaborating features in GitHub so I can invite a real front end designer to have a look at my attempts to customize the theme. My last step is to do a Sync again in Appernetic and then a Publish and after 10 min all is live on [GitHub Pages][6].

From now on it is very easy to start blogging. Select the post directory in the tree view, it is where blog post lives. Create a new file,  name it with a headline, it will be sluggified automatically.Select toml or yaml front matter (toml as default selection),. The file tree will be updated and show the new file. Open the file and blog! Turn on auto save and all text you write will be saved every one minute. Remember to undraft the post if you would like to see it after publishing. 

![enter image description here][7]

Happy blogging!
  [1]: /images/themes-opt.png
  [2]: https://appernetic.io
  [3]: https://github.com/mmrath/hugo-bootstrap
  [4]: /images/Sync-opt.png
  [5]: /images/githubdesktop-opt.png
  [6]: https://appernetic.github.io/
  [7]: /images/Startblogging.png
