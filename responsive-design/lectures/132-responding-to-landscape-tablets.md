# 132. Responding to Landscape Tablets

1200px the design/layout not breaking but at 100% view everything looks too big. To fix this we can add breakpoint at 122px.

First we make use of responsive units. To make everything smaller on the page we change the `html` font size:

```html
html { font-size: 62.5%; }
```

## Re-size Headings

Make the secondary and tertiary haedings smaller as well. Also reduce the spacing between columns within our grid.

### Propteries

Refer to other two css files and make some layout chances.

Target these properties:
`.heading-secondary`
`.heading-tertiary`
`.header`
` .main-nav-list`

Reduce the column gap within the hero section which is the first section on the page.
`.hero`

Add padding to the left and right of the testimonials container
`.testimonials-container`
