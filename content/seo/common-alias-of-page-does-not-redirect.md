When publishing your website you need to decide if you will be using the www pre-fix or not:

```
server {
	# either
	server_name example.com;
	# or
	server_name www.example.com;
}
```

From an SEO perspective it doesn't matter which one you choose. What is important is that you do not publish on both. 


<!-- The following heading is enforced by the interpreter -->
# How do I fix this ?

You need to add an HTTP 301 redirect on the option that you will *not* be using:

```
server {

		# redirect www to our non www domain
        server_name www.example.com;
        return 301 $scheme://example.com$request_uri;

        # OR

        # redirect non www to our www domain
        server_name example.com;
        return 301 $scheme://www.example.com$request_uri;

}
```

This will ensure that your content only gets published on your chosen option.
It will also stop split search engine rankings.

# Practical argument for no www 

Naked domains use less characters and get rid of cruft that is mostly unnecessary.
This may make a real difference when your domain is used or linked to by a character limited service.
Use naked domains if you're into brevity and all that.

# Technical argument for using www

Cookieless domains present a reason for using www. 
By using a prefixless domain, cookies get served even on your subdomains.
If you want to serve static assets from lets say assets.example.com it will still have cookies.

# Resources

* [blog.stackoverflow.com](https://blog.stackoverflow.com/2008/06/dropping-the-www-prefix/)
* [sitepoint](http://www.sitepoint.com/domain-www-or-no-www/)
