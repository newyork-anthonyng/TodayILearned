```html
<a href="./link/to/image.png">Download</a>
```

You have a link to an image. When you click it, the browser opens the image.

But what if you want to download the image?

HTML5 has provides a `download` attribute.

```html
<a href="./link/to/image.png" download>Download</a>
```

> When used on an anchor, this attribute signifies that the browser should download the resource the anchor points to rather than navigate to it.

However, this only works with same-origin assets. If your asset is located on another domain, the `download` attribute does not work.

Another way to do this is to make server-side changes. The `Content-Disposition` header for a resource defaults to `inline`. This indicates that this resource should be displayed inside the web page.

You can set `Content-Disposition` to `attachment`. This indicates that the browser should download the resource.

[MDN Reference for Content-Disposition](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Disposition)
