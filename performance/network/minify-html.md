Minification refers to the process of removing unnecessary or redundant data without affecting how the resource is processed by the browser - e.g. code comments and formatting, removing unused code, using shorter variable and function names, and so on.

Minified HTML helps reduce bandwidth usage and is more effective with Gzip. 


# How do I fix this ?

Use a build tool (`npm`, `grunt` or `gulp`) to automate the minification of your production javascript and css (but also keep the development files in human readable format). Alternatively, command-line and online minifiers also exist.


# Resources

* [html-minifier](https://www.npmjs.com/package/html-minifier)
* [HTML Minifier](https://kangax.github.io/html-minifier/)
* [gulp-htmlmin](https://github.com/jonschlinkert/gulp-htmlmin)
* [Google Developers - Minify Resources](https://developers.google.com/speed/docs/insights/MinifyResources?hl=en)
* [Effects of GZipping vs. minifying HTML files](http://madskristensen.net/post/effects-of-gzipping-vs-minifying-html-files)
