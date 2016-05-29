+++
author = "author"
date = "2016-02-18T20:27:25Z"
description = "If you just have set up your Appernetic account you need to add a theme. The easiest way is to clone a theme which you can do from the drop down button beside the blue Preview button to the right."
draft = false
keywords = ["Static", "Blogging", "GitHub","static website"]
tags = ["Static web site generator", "Blogging", "GitHub","static website"]
title = "Collaborating and working with hugo themes"
topics = ["static website"]
type = "post"

+++
## Customizing themes
If you just have set up your Appernetic [static website service][1] account you need to add a theme. The easiest way is to clone a theme which you can do from the [menu button][2]. 

![Install a theme][3]

You can start by cloning my customized [hugo-bootstrap theme][4] or get one from [Hugo][5]. Then select the theme from the list of themes and click Use Theme. When you do that the theme config settings will be copied to your project folder. Now open the settings tab and change the settings as you would like to have it.

You can change the bootswatch to another design by changing the theme = "paper" under [params].

Here is the different bootswatch designs you can use:

 - cerulean
 - cosmo
 - cyborg
 - darkly
 - default
 - flatly
 - journal
 - lumen
 - paper
 - readable
 - sandstone
 - simplex
 - slate
 - spacelab
 - superhero
 - united
 - yeti 

There are lots of themes at [Hugo][6], but you probably want to customize the theme before you use it so that you have a blog with  a theme that is matching your business website or service. I am using Bootswatch Paper theme for [Appernetic static website service][7]. Fortunately, I found [hugo-bootstrap][8] and cloned it. 

![enter image description here][9]
Now you can also browse the [theme showcase gallery][10].

Then to customize it further I pressed the **Sync** button which does a pull and then a push to your Appernetic project repository at [GitHub][11] with the name **appernetic-hugo-project** . When you start out you will not have this repo so it is automatically created for you and all strange git commands is hidden away so you do not have to think about it.

> When you start out you will not have this repo so it is automatically
> created for you and all strange git commands is hidden away so you do
> not have to think about it.

![Sync with GitHub][12]

Now to work with the theme I did a pull to my local computer, edited the theme with my favorite editor *Atom* and after that I did a commit and a push back to my GitHub project repo. If you are a hard-core git user you would start terminal and add the commands. There is also a very easy to use desktop client for [GitHub][13].

![GitHub Desktop app][14]

## Collaborating 
Notice also that I have all the social and collaborating features in GitHub so I can invite a real front end designer to have a look at my attempts to customize the theme. My last step is to do a **Sync** again in Appernetic and then a **Publish** and after 10 min all is live on [GitHub Pages][15].

> Notice also that I have all the social and collaborating features in
> GitHub so I can invite a real front end designer to have a look at my
> attempts to customize the theme.

## Start blogging!
From now on it is very easy to start blogging. Select the **post** directory in the tree view, it is where blog post lives. Create a new file,  name it with a headline, it will be sluggified automatically. Select *TOML* or *YAML* front matter (TOML as default selection). The file tree will be updated and show the new file. Open the file and blog away! Turn on auto save and all text you write will be saved every other minute. Remember to **undraft** the post if you would like to see it after publishing and  add key words, tags, and topics.

![Start blogging][16]

Happy blogging!

Tip, skip the first headline in the post (at least in hugo-bootstrap it will be added automatically) and edit the *front matter* located at the bottom of the editor after the preview and switch the first letter in the title to capital.
 


  [1]: https://appernetic.io
  [2]: https://appernetic.io/app/#/dashboard/list/themes
  [3]: https://res.cloudinary.com/appernetic/v1457304135/pig3qgwntchbkk0x9tab
  [4]: https://github.com/appernetic/hugo-bootstrap-mod.git
  [5]: http://themes.gohugo.io/
  [6]: http://themes.gohugo.io/
  [7]: https://appernetic.io
  [8]: https://github.com/mmrath/hugo-bootstrap
  [9]: https://res.cloudinary.com/appernetic/v1464371347/mgc1lnbrytafkitsjmma
  [10]: https://blog.appernetic.io/2016/05/27/appernetic-theme-showcase-gallery/
  [11]: https://github.com/
  [12]: https://res.cloudinary.com/appernetic/v1457304341/htdhjub2yfcw4bpkzklw
  [13]: https://desktop.github.com/
  [14]: https://res.cloudinary.com/appernetic/v1457304455/tdsbe75348lm3dxa1csw
  [15]: https://appernetic.github.io/
  [16]: https://res.cloudinary.com/appernetic/v1457304529/clqxr6v6xhxum0jvqabz
