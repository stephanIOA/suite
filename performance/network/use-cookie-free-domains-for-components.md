From a performance perspective, the trouble with cookies is that once the server sets a cookie for a particular domain, all subsequent HTTP requests for that domain must include the cookie.  Even if the server has no use for the cookie, as is usually the case with static components, the cookie is sent over the wire anyway, bloating our request headers with useless code.

# How do I fix this ?

When the server sets a cookie, that cookie is attached to all future requests to the **same domain** (and often all subdomains as well). To get around this we simply need to request our static assets from a different domain.

The easiest way to set up a cookieless domain for your static content is to create a CNAME record aliasing your static domain to your main domain. Your static files remain in the same place, but you can now reference them at a different domain.

# Resources

* [Static cookieless domain](http://www.ravelrumba.com/blog/static-cookieless-domain/)
