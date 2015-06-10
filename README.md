# lucifer
responsive css and javascript framework for web theme coding

Everything you need before starting using lucifer is how to code in SASS, download lucifer and unzipp it in your project. Yep, that’s all. Sure, if you don’t know how to code in SASS, we recommend you SASS documentation and the Koala compiler.

For better understanding of the structure of lucifer let’s go step by step through it.

INSTALL
<br>Download the lucifer compressed file and unzipp it in your project.

LOAD PARTS
<br>There is a file named settings.sass for loading components and modules you need and looks like this:

```// settings.sass
 
/* including resources */
<br>@import resources/normalize.css
 
*, *:before, *:after
<br>	box-sizing: border-box
 
// including libs
<br>@import lib/functions.sass
<br>@import lib/unification.sass
<br>@import lib/mixins.sass
<br>@import lib/grid.sass
<br>@import lib/typography.sass
 
// including components
<br>@import lib/components/gradient.sass
<br>@import lib/components/icons.sass
<br>@import lib/components/arrow.sass
<br>@import lib/components/list.sass
<br>@import lib/components/table.sass
<br>@import lib/components/tabs.sass
<br>@import lib/components/breadcrumbs.sass
<br>@import lib/components/tooltip.sass
<br>@import lib/components/rating.sass
<br>@import lib/components/switcher.sass
<br>@import lib/components/radiocheckbox.sass
 
// setting defaults
<br>$fontsList: (("abrilfatface", "fonts/abrlfatface-regular-webfont"), ("anton", "fonts/anton-webfont"))
 
/* load fonts */
<br>+loadFonts($fontsList)
 
<br>// custom code
<br>...```

As you can see, you could import whatever component you want and do not include what you dont want to and what you will not use as well. We highly recommend you to include these files:

* functions.sass
* unification.sass
* mixins.sass

because there are some components that use functions and mixins from these files to work.

You could find more informations about this library in the location [http://lucifer.technology/](http://lucifer.technology/ "http://lucifer.technology/").
