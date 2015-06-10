# lucifer
responsive css and javascript framework for web theme coding

Everything you need before starting using lucifer is how to code in SASS, download lucifer and unzipp it in your project. Yep, that’s all. Sure, if you don’t know how to code in SASS, we recommend you SASS documentation and the Koala compiler.

For better understanding of the structure of lucifer let’s go step by step through it.

INSTALL
<br>Download the lucifer compressed file and unzipp it in your project.

LOAD PARTS
<br>There is a file named settings.sass for loading components and modules you need and looks like this:

```sass
// settings.sass
 
/* including resources */
@import resources/normalize.css
 
*, *:before, *:after
	box-sizing: border-box
 
// including libs
@import lib/functions.sass
@import lib/unification.sass
@import lib/mixins.sass
@import lib/grid.sass
@import lib/typography.sass
 
// including components
@import lib/components/gradient.sass
@import lib/components/icons.sass
@import lib/components/arrow.sass
@import lib/components/list.sass
@import lib/components/table.sass
@import lib/components/tabs.sass
@import lib/components/breadcrumbs.sass
@import lib/components/tooltip.sass
@import lib/components/rating.sass
@import lib/components/switcher.sass
@import lib/components/radiocheckbox.sass
 
// setting defaults
$fontsList: (("abrilfatface", "fonts/abrlfatface-regular-webfont"), ("anton", "fonts/anton-webfont"))
 
/* load fonts */
+loadFonts($fontsList)
 
// custom code
...
```

As you can see, you could import whatever component you want and do not include what you dont want to and what you will not use as well. We highly recommend you to include these files:

* functions.sass
* unification.sass
* mixins.sass

because there are some components that use functions and mixins from these files to work.

You could find more informations about this library in the location [http://lucifer.technology/](http://lucifer.technology/ "http://lucifer.technology/").
