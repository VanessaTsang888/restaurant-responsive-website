# 119 Building the Testimonials Section - Part 2

Add the Gallery to the Testimonial section using the power of CSS3.

- 12 images
- Gallery will be our grid container.
- The `<figure>` element is the perfect element for images, example in a blog post images and usually they also have a caption such as the `<figcaption>` element.

## Images

They are inline element by default and we'll make them block element to remove the defeault gaps between the images.

## Styling and layout

To remove the default gaps between each image by set to block level element.

```css
// Use the desendand selector `img`as the class is inside that selector
.gallery-item img {
  display: block;
}
```

### Create our grid

This is instead of using our pre-defined grid.

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
// Make the images flexible so they fit within the grid.
.gallery-item img {
  display: block;
  width: 100%;
}
```

Add small spacing between each image using the `gap` property.

## Change background colour

Change backgraound colour from white to light orange as this is a different section to the previous section.

## More Spacing

The top and right side spacing need to be the same of the spacing between that is between each image.

## Colour of testimonial-name

Need to change the `testimonial-name` text colour that is on the light orange background to meet the colour constrast ratio on the digital accessibility guidelines: [WCAG 2.1 - Contrast (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html).

Use the [contrast check tool](https://webaim.org/resources/contrastchecker/) as the WCAG guidelines has suggested.

## Image effect

Scale-in effect on-hover but without them overflowing.
Use existing class od `.gallery-item` and use the css pseudo class of hover on it: `.gallery-item img:hover`. Use the property of `transform` to scale each image by 1.1 value. ON the `.gllery-item` class we don't want any overflow so we need to hide it. The transition on each image will be just 0.4 seconds.
