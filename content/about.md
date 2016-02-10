+++
author = "author"
date = "2016-02-10T20:21:11Z"
description = "description"
draft = false
keywords = ["key", "words"]
tags = ["one", "two"]
title = "about"
topics = ["topic 1"]
type = "post"

+++
#Front Matter
Now you can select yaml or toml front matter when you create a new file.

If you don't select front matter, default settings is to create a toml file.

We don't support json front matter yet. It conflicts heavilly with Restangular, so that needs to be investigated a little bit before implementing.

If the front matter can't be detected because there is no or wrong format set in config.toml we leave the md file as is. Therefore you will se some strange code in the PageDown editor.
