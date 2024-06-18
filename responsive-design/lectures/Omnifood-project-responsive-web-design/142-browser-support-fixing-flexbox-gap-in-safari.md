# Lecture 142. Browser Support and Fixing Flexbox Gap in Safari

The Process Behind Building A Website:

5. Test And Optimise

-> Make sure website works well in all major browsers - Chrome, Firefox, Safari, Edge, maybe even old IE.

-> Test the website on actual mobile devices, not just in DevTools.

-> Optimise all images, in terms of dimensions and file size - see lecture on images.

-> Fix simple accessibility problems, e.g. color contrast issues.

-> Run the Lighthouse performance test in Chrome DevTools and try to fix reported issues.

-> Think about Search Engine Optimisation (SEO).

## Browser Support

How different browsers support different CSS properties. Today most browsers support the most important CSS properties. However, there are some users still using older browsers like the older version of IE or stuck on some older Safari version.

Find out what the browser support is like for css grid with this resource:
[Can I use](https://caniuse.com/) -> search by css property such as css grid, flexbox etc.
We can see all the modern browsers support it.

### Vendor Prefixes

Use vendor prefixes to make a CSS property work accross multiple browsers.
For backdrop filter css property will work on Safari but only with `-webkit-`

`backdrop-filter` blurs everything that is behind that element. In our case we use background-color of 60%. This works in Chrome but not in Safari without `-webkit-`.

`-webkit-backdrop-filter` property with value of `blur(5px)`.

Edge uses -webkit- too.

## Fix Flexbox Gap property in Safari browsers

script.js

// Fixing flexbox gap property missing in some Safari versions

Include this func in our code `function checkFlexGap()` for the next couple of years.

### queries.css

The new code at the bottom of this file:
For every instance where we used the gap property together with Flexbox.
