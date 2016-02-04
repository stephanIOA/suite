Invalid link type was found for attribute `rel` in `a` tag. HTML5 only allows you to use the standard link types without registering a new type.

```html
<a href="sample.html" rel="non-existing-linktype">Sample Link</a>
```

# How do I fix this ?

Use a standard link type:
* alternate
* author
* bookmark
* help
* license
* next
* nofollow
* noreferrer
* prefetch
* prev
* search
* tag

```html
<a href="sample.html" rel="alternate">Sample Link</a>
```

# Resources

* [W3C - Link Types](https://www.w3.org/TR/html5/links.html#linkTypes)
* [W3C - Other Link Types](https://www.w3.org/TR/html5/links.html#other-link-types)
