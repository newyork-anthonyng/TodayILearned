In HTML, you use script tags like so:
```html
<script src="http://some-important-script.js">
```

However, if your website is on `https`, and you request a resource over `http`, your browser will complain.

> [See Mixed Content](https://developers.google.com/web/fundamentals/security/prevent-mixed-content/what-is-mixed-content)

One work-around is to leave the protocol out of the URL:
```html
<script src="//some-important-script.js">
```

The browser will call the resource based on the protocol of your website. For example:
* If your website is `https`, it will call `https://some-important-script.js`
* If your website is `http`, it will call `http://some-important-script.js`

# References

* https://stackoverflow.com/questions/550038/is-it-valid-to-replace-http-with-in-a-script-src-http
* https://stackoverflow.com/a/14832916/6241383
* https://en.wikipedia.org/wiki/URL#Protocol-relative_URLs
