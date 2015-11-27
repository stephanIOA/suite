Since favicon.ico resides in the server's root, each time the browser requests this file, the cookies for the server's root are sent. Making the favicon small and reducing the cookie size for the server's root cookies improves performance for retrieving the favicon.

Making favicon.ico cacheable avoids frequent requests for it.

# How do I fix this ?

* Make the favicon as small as possible (preferably under 1kb)
* Rather use `<link rel="apple-touch-icon" href="..."> png's for larger icon sizes
* Set `Expires` header far into the future

# Resources

* [GTmetrix - Make Favicon small and cacheable](https://gtmetrix.com/make-favicon-small-and-cacheable.html)
