+++
author = "author"
date = "2016-02-18T20:27:25Z"
description = "description"
draft = false
keywords = ["Static", "Blogging", "GitHub"]
tags = ["Static web site generator", "Blogging", "GitHub"]
title = "Collaborating and working with hugo themes"
topics = ["topic 1"]
type = "post"

+++
## Customizing themes
If you just have set up your Appernetic account you need to add a theme. The easiest way is to clone a theme which you can do from the drop down button beside the blue **Preview** button to the right. 

![enter image description here][1]

Thou there is lots of themes at [Hugo][2], you probably want to customize the theme before you use it so that you have a blog with  a theme that is matching your business web site or service. I am using Bootswatch Paper theme for [Appernetic service][3]. Fortunately I found [hugo-bootstrap][4] and cloned it. 

Then to customize it further I pressed the **Sync** button which does a pull and then a push to your Appernetic project repository at [GitHub][5] with the name **appernetic-hugo-project** . When you start out you will not have this repo so it is automatically created for you and all strange git commands i hidden away so you do not have to think about it.

> When you start out you will not have this repo so it is automatically
> created for you and all strange git commands i hidden away so you do
> not have to think about it.

![enter image description here][6]

Now to work with the theme I did a pull to my local computer, edited the theme with my favorite editor *Atom* and after that I did a commit and a push back to my GitHub project repo. If you are a hard-core git user you would start terminal and add the commands. There is also a very easy to use desktop client for [GitHub][7].

![enter image description here][8]

## Collaborating 
Notice also that I have all the social and collaborating features in GitHub so I can invite a real front end designer to have a look at my attempts to customize the theme. My last step is to do a **Sync** again in Appernetic and then a **Publish** and after 10 min all is live on [GitHub Pages][9].

> Notice also that I have all the social and collaborating features in
> GitHub so I can invite a real front end designer to have a look at my
> attempts to customize the theme.

## Start blogging!
From now on it is very easy to start blogging. Select the **post** directory in the tree view, it is where blog post lives. Create a new file,  name it with a headline, it will be sluggified automatically. Select *toml* or *yaml* front matter (toml as default selection). The file tree will be updated and show the new file. Open the file and blog away! Turn on auto save and all text you write will be saved every one minute. Remember to **undraft** the post if you would like to see it after publishing and add

![enter image description here][10]

Happy blogging!

Tip, skip the first headline in the post (at least in hugo-bootstrap it will be added automatically) and edit the *front matter* located at the bottom of the editor after the preview and switch the first letter in the title to capital and add key words, tags and topics.
 


  [1]: /images/themes-opt.png
  [2]: http://themes.gohugo.io/
  [3]: https://appernetic.io
  [4]: https://github.com/mmrath/hugo-bootstrap
  [5]: https://github.com/
  [6]: /images/Sync-opt.png
  [7]: https://desktop.github.com/
  [8]: /images/githubdesktop-opt.png
  [9]: https://appernetic.github.io/
  [10]: /images/Startblogging.png
