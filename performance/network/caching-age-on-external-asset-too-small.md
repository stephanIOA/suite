One or more of your external assets have an extremely short cacheing age. This nullifies the point of allowing the browser to store resources for future use.

# How do I fix this ?

If possible, set an expires heading for at least two days in the future. If the headers can't be changed, because the server is controlled by a third party, consider hosting the file yourself (on a CDN, if possible).

# Resources

* [Webmasters Stackexchange - Cace external static scripts (http://webmasters.stackexchange.com/questions/16534/cache-external-static-scripts)
