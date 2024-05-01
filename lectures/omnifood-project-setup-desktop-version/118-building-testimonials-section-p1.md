# 118. Building the Testimonials Section - Part 1

Building Testimonials and Gallery section.

This section will full up the enitre available width called a full bleed section.

Left side: 2 by 2 grid.
Right side: gallery of photos.

## Code

HTML code:
New section tag but not within a container to centre the context in the page. Instead we'll 2 boxes, one for the Testimonials and one for Gallery.
We want these two side by side so we use our grid class within the section tag.

```css
.grid .grid--2-cols;
```

Test in UI:
Reload the browser mannually to test on screen.

Blockquotes:

The blockquotes tag represent quotes - things that someone else said. Testimonials is exactly this.

## Layout

Put the x4 customers in a 2 by 2 grid:

- write new styles rather the reusable grid we used before but the spacing on that one is not ideal as its for the overal layout and too big for this small component.

Images:
make them a fixed width. Since the images are square, the height will auto be figured out by the browser. Make them round by using the `border-radius` property.

Testimonial name:
Lighter in colour as it less important. In terms of the colour ratio, we'll come back later to work on that.
