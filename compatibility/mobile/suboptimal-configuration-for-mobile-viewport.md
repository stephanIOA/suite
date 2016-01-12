The viewport controls how your webpage is rendered on mobile devices. If no viewport is specified mobile devices will try to render with typical desktop width for compatibility which breaks user experience.

To avoid problems with screen sizes it's not recommended to specify explicit widths for the viewport.

When checking for the viewport we expect to see the following:

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

in the `<head>` of your page. This will render pages optimized to display well on mobile devices with the full width of the device viewport.

# How do I fix this ?

To fix ensure that the correct viewport supplied is configured correctly.

# Resources

* [Google Pagespeed Insights](https://developers.google.com/speed/docs/insights/ConfigureViewport?hl=en)
