
## Organizing Content Using Sections
Sections allow you to group content by 'type', and determines how they are displayed.
For example, all blog posts follow the same format, so they are stored within the same section.

For file organization purposes you can create a section that is rendered and grouped
	together within another section. For this to work, each piece of content needs
	to specify its `type` as that of the other section.
```
content/
	blog/
		first-post.md
	travel-blog/
		trip-to-mars.md
```
```
trip-to-mars.md:
	+++
	type = "blog"
	+++

	...
```

## Organizing Content Using Taxonomies
A `Taxonomy` is a "type of label" used to provide classification for content across `sections`.
Examples of Taxonomies are `Category`, `Tag`, `Author`, and `Series`.
(`Date` could even be considered as a Taxonomy.) Each Taxonomy groups the content by `terms`.

Categories should generally be limited to a small set of general terms like:
	`News`, `Random`, `Technology`. A piece of content should rarely belong to more than two Categories.

Tags are a much more fine-grained mechanism to add metadata to content.
These generally don't provide much benefit, but if you do use them, try to be
	consistent to prevent tags from only linking to a singular content piece.

The `Author` Taxonomy allows you to find or subscribe to content written by a specific author.
Due to Hugo's implementation, the `author` parameter within a content's front matter
	must be an array of terms, even though only one author is needed(hugo-plus only support one).

To customize the Author, Project, or Series Taxonomy pages, [read this section](#custom-taxonomy-and-term-pages).


### Creating Your Own Taxonomy
If you need to create your own Taxonomy to classify content across sections
	that `hugo-plus` let us know.


## Overview of Templates
Hugo's documentation on templates can be found [here](http://gohugo.io/templates/overview/)

Templates are used to build HTML pages for the different types of Hugo pages:
	`section`, `taxonomy`, `terms`, `single`, `list` as well as the different
	types of `content views`: `summary` and `li`.
	Default implementations of these templates are found within `layouts/_default/`.

Templates are composed of smaller templates called `partials` located within `layouts/partials/`.
Partials are used to define reusable template components that multiple templates
	share, for example, a site's sidebar, navbar, or footer.

Some components can be enabled/disabled on a per-section basis by setting
	parameters for that section within `data/section/<section name>.toml`.
	For example, you can disable comments for content within the author section
		by setting `no_comments = true` within `data/section/author.toml`.

Other templates use site-wide parameters defined within the `config.toml` file.
	These configurations include navigation bar links and menus, social links
		for the site, footer text, date format for posts, theme, site
		description, etc.

See [this page](Parameters.md) full documentation of the pre-defined parameters.
	

### How is the Site Built?
* A template within `layouts/_default/` corresponding to the current page is
	processed
* This template first includes `/layouts/partials/header.html` which includes
	the dependencies of Themes, Layouts, and Plugins.
* The Section's Layout is found its `template` file is processed
* The Layout's template establishes the main HTML structure, reads the Components
	within the Layout containers, checks if their disabled, then loads them
* Finally, it includes `/layouts/partials/footer.html` which processes
	`body_inline` template dependencies.


## Customizing the Bootstrap Theme's Look and Feel
Bootstrap is used as the foundation due to its ubiquity.

There are many themes available for free, but you may want to create
your own or customize an existing one.

If you google `bootstrap theme editor` you can find an editor that allows you
create your own theme. Some also allow you to download the `variables.less`
file which is used to compile into the final css file. This can be useful if
you want to modify the theme in the future.

### Compiling and Customizing Bootstrap From Source
Bootstrap is written using Less, which is then compiled into CSS.
Before we continue, you'll need to setup the toolchain.

First you'll need to [install nodejs](http://nodejs.org/download/).

Once, nodejs is setup, The Less compiler can installed using `npm`. (May require admin privileges.)
> npm install -g less

The source files for Bootstrap and the hugo-plus theme is stored within the 
`util/` directory.
Most changes to the theme can done within `bootstrap/variables.less`.

To compile the less into css and apply it to the website, run:
> lessc --compress hugo-plus.less > ../static/css/hugo-plus.min.css

If you are on Linux, the `listen.sh` script will recompile the theme
whenever the `bootstrap` folder is updated.


