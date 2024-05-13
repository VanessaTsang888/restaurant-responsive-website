# 131 Responding to Small Laptops

For responsive web design the viewport is very important as without the new meta tag code responsive web design will not work on physical mobile devices as browsers on mobile devices will auto zoom the page out by default until it fits the screen. This is not what we want with media queries as we simply want to make our entire design smaller, less wide.

```html
<!-- The viewport is very important for responsive web design -->
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

This meta tag code will make it so that the page will match the screen's width.

The page width will be equal to the deice width.
`content="width=device-width`

The scale initially should be 100%.
Will not zoom out of the page to fit on the screen.
`initial-scale=1.0"`

## Set our media queries

To write our media queries we need our breakpoints which is the width that we want to set the media queries. So we use the two methodologies we studied in last lecture which is looking where our design breaks and also taking into account common screen width ranges.

Looking where our design breaks and taking into account common screen width ranges.

Common screen size called HD ready: 1366px. Set our first breakpoint here.
In media queries we don't use pixels like we do with our layouts as using pixels will not adjust with user font size settings in the browser.

rem and em do NOT depend on html font-size in media queries! Instead, 1rem = 1em = 16px.
So rem is the root font size and em is the current font size.
rem has bugs in some browsers when used in media queries. Therefore, we should em rather than rem.

Breakpoint 1350px. Convert to em: 1350 / 16 = 84,375. We can round that off to 84 -> 84em.
84 \* 16 = 1344px

Our first media query with first breakpoint:

```css
/* Below 1344px (Smaller desktops) */
@media (max-width: 84em) {
  ...;
}
```

Write our first css rule in the above media query.
The rem within the css rule has nothing to do with the em and it works as before.

```css
/* Below 1344px (Smaller desktops) */
@media (max-width: 84em) {
  .hero {
    max-width: 120rem;
  }
}
```

Now the hero section has the same width as the content in the sections below it. Now we have new problem that the heading is on 4 lines. To fix it we need to decrease the value of the font-size.

```css
@media (max-width: 84em) {
  .hero {
    max-width: 120rem;
  }
  .heading-primary {
    font-size: 4.4rem;
  }
}
```

Lets not add a media query to fix every problem as that will be an over kill. But for the Gallery we need to now change the 3 columns to 2 columns.

```css
@media (max-width: 84em) {
  .hero {
    max-width: 120rem;
  }
  .heading-primary {
    font-size: 4.4rem;
  }
  .gallery {
    grid-template-columns: repeat(2, 1fr);
  }
}
```

## Next up

Next lecture we will create our next breakpoint.
