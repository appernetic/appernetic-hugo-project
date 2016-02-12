
# Gallery Lightbox Popup
This Shortcode groups the following Shortcodes together into a Gallery:
	* photo, video, iframe, popup

# Usage
```
	{{% gallery %}}
		{{% photo src="/image/test.png" title="This is just a test" %}}
		{{% photo src="image/test2.png" title="Another test" %}}
		{{% video src="youtu.be/hugo" title="Video test" %}}
	{{% /gallery %}}
```

# Parameters
* id - Id attribute for gallery's out `div` tag
* class - Class attribute for gallery's out `div` tag
* style - Style attribute for gallery's out `div` tag

# Todo
* config - Configuration file found within `.Site.Data`('data' directory)
	* This could only work if magnific js code was included here,
		'magnific-gallery' class attribute was removed, and the `id`
		attribute is set.(maybe use src as an id instead?)

