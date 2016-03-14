hugo-bootstrap-mod
==================
A theme with bootstrap, bootswatch(optional), font-awesome, highlightjs

*NOTE: This theme is copied from Hyde-Y. Not everything is ported to bootstrap.
Feel free to make changes and open pull requests.*


<small>Forked from [Hyde-Y](https://github.com/enten/hyde-y)</small>

Here you check out Appernetic's blog site using this [theme](https://appernetic.github.io/).

## Screenshots

![preview](https://raw.githubusercontent.com/appernetic/hugo-bootstrap-mod/master/images/screenshot2.png)

Hugo-bootstrap-mod theme used with ```showRightSidebar = true``` and ```[params.theme] name = "paper"``` .


![preview](https://raw.githubusercontent.com/appernetic/hugo-bootstrap-mod/master/images/screenshot.png)

Hugo-bootstrap-mod theme with default settings.


## Installation with Appernetic Static Site Generator as a Service

1. Click the arrow to the left of the blue "Preview" button up to the right, select "Themes".
2. At the bottom of the Themes page paste the git link from GitHub (see image fig 1).
3. If you want to update your config settings file click the "Use" button in the theme modal popup (WARNING! The current settings file will be overwritten), otherwise follow step 4.
4. In Settings change the line theme = "theme-name-here" to theme = "hugo-bootstrap-mod"
5. To configure menues and footer you need access to the data folder, read more in section "Access data folders". 
5. Click the button: Preview or Publish
6. Wait 10 min or clear your local browser cache to see changes at GitHub. In preview content is updated imediatley but CSS changes need a cache clear to be visible.  


![preview](https://raw.githubusercontent.com/appernetic/hugo-bootstrap-mod/master/images/cloneatheme.png)

Figure 1. Copy git link from GitHub.

## Access data folders

In Appernetic.io you only have access to the Content folder and the config settings file. 

To access the data folder you have two options:

Option 1

1. First fork this theme repo.
2. Find the data folder and add a Menu.toml file.
2. Clone your forked repo in Appernetic.io

Option 2

1. Fork this repo.
2. Use Git or GitHub Desktop on your local computer to clone your forked theme repo.
3. Create a Menu.toml file in your data folder with you favorite editor.
4. Sync with your GitHub theme repo.

## Installation with Hugo

```
$ cd your_site_repo/
$ mkdir themes
$ cd themes
$ git clone https://github.com/mmrath/hugo-bootstrap
```

See the [official Hugo themes documentation](http://gohugo.io/themes/installing) for more info.

## Usage 

This theme expects a relatively standard Hugo blog/personal site layout:
```
.
└── content
    ├── post
    |   ├── post1.md
    |   └── post2.md
    ├── code
    |   ├── project1.md
    |   ├── project2.md
    ├── license.md        // this is used in the sidebar footer link
    └── other_page.md
```

Just run `hugo --theme=hugo-bootstrap` to generate your site!

## Configuration (Applies to Appernetic.io also)

### Hugo 

An example of what your site's `config.toml` could look like. All theme-specific parameters are under `[params]` and standard Hugo parameters are used where possible.

``` toml
# hostname (and path) to the root eg. http://spf13.com/
baseurl = "http://www.example.com"

# Site title
title = "sitename"

# Copyright
copyright = "(c) 2015 yourname."

# Language
languageCode = "en-EN"

# Metadata format
# "yaml", "toml", "json"
metaDataFormat = "yaml"

# Theme to use (located in /themes/THEMENAME/)
theme = "hugo-bootstrap"

# Pagination
paginate = 10
paginatePath = "page"

# Enable Disqus integration
disqusShortname = "your_disqus_shortname"

[permalinks]
    post = "/:year/:month/:day/:slug/"
    code = "/:slug/"

[taxonomies]
    tag = "tags"
    topic = "topics"

[author]
    name = "yourname"
    email = "yourname@example.com"

#
# All parameters below here are optional and can be mixed and matched.
#

# bootswatch theme name, unmark and select one: cerulean, cosmo, cyborg, darkly, 
# default, flatly, journal,  lumen, paper, readable, sandstone, simplex, 
# slate, spacelab, superhero, united, yeti. 
#[params.theme]
#  name = "paper"
  
[params]
    # You can use markdown here.
    brand = "foobar"
    topline = "few words about your site"
    footline = "code with <i class='fa fa-heart'></i>"

    # Show a sidebar menu
    showRightSidebar = true

    # Text for the top menu link, which goes the root URL for the site.
    # Default (if omitted) is "Home".
    home = "home"

    # Select a syntax highight.
    # Check the static/css/highlight directory for options. 
    highlight = "default"

    # Google Analytics.
    googleAnalytics = "Your Google Analytics tracking code"

    # Sidebar social links.
    github = "enten/hugo-boilerplate" # Your Github profile ID
    bitbucket = "" # Your Bitbucket profile ID
    linkedin = "" # Your LinkedIn profile ID (from public URL)
    googleplus = "" # Your Google+ profile ID
    facebook = "" # Your Facebook profile ID
    twitter = "" # Your Twitter profile ID
    youtube = ""  # Your Youtube channel ID
    flattr = ""  # populate with your flattr uid

[blackfriday]
    angledQuotes = true
    fractions = false
    hrefTargetBlank = false
    latexDashes = true
    plainIdAnchors = true
    extensions = []
    extensionmask = []

```

### Menu

Create `data/Menu.toml` to configure the top menu navigation links. Example below.

```toml
[about]
    Name = "About"
    IconClass = "fa-info-circle"
    URL = "/about"

[posts]
    Name = "Posts"
    Title = "Show list of posts"
    URL = "/post"

[tags]
    Name = "Tags"
    Title = "Show list of tags"
    URL = "/tags"
```

### Foot menu

Create `data/FootMenu.toml` to configure the footer navigation links. Example below.

```toml
[license]
    Name = "license"
    URL = "/license"
```

## Tips

* If you've added `theme = "hugo-bootstrap"` to your `config.toml`, you don't need to keep using the `--theme=hugo-bootstrap` flag!
* Although all of the syntax highlight CSS files under the theme's `static/css/highlight` are bundled with the site, only the one you choose will be included in the page and delivered to the browser.
* Change the favicon by providing your own as `static/favicon.png` (and `static/touch-icon-144-precomposed.png` for Apple devices) in your site directory.
* Hugo makes it easy to override theme layout and behaviour, read about it [here](http://gohugo.io/themes/customizing).
* Pagination is set to 10 items by default, change it by updating `paginate = 10` in your `config.toml`.

## Changes and enhancements from the original theme

* Modified to work with bootstrap and bootswatch
* ...many other small layout tweaks!

## Attribution

Obviously largely a port of the awesome [Hyde-Y](https://github.com/enten/hyde-y) theme.

## Questions, ideas, bugs, pull requests?

All feedback is welcome! Head over to the [issue tracker](https://github.com/mmrath/hugo-bootstrap/issues).

## License

Open sourced under the [MIT license](https://github.com/enten/hyde-y/blob/master/LICENSE).
