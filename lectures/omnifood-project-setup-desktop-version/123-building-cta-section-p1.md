# 123. Building the Call-To-Action Section - Part 1

html elements with temp content to test in UI.

## Building the content

```html
<section class="section-cta">
  <div class="container">
    <div class="cta">CTA</div>
    <div class="cta-text-box">IMAGE</div>
    <div class="cta-img-box" role="img" aria-label="Woman enjoying food"></div>
  </div>
</section>
```

## CSS3: styles and layout

We never want a dark shadow.
Gradient: `linear-gradient` to the right bottom

- this means flow from top-left corner to bottom-right corner

### Image

Move out of the css directory, into the root directory and into the image directory. The x2 periods means go to the parent directory, moving one level up in the file tree.

```css
    url('../img/eating.jpg');
```

Class `.cta-img-box`
Background image is too bright so to visually set the image back we use colours to layover the image and on opacity/transparency.

```css
/* The image is overlaping the cta element. To fix this use the overflow property.  */
.cta {
  overflow: hidden;
}
```

#### Digital Accessibility

```html
<!-- The content is in css not html so for screen readers we need the html role and the aria-label properties -->
<div class="cta-img-box" role="img" aria-label="Woman enjoying food"></div>
```

So we use the `aria-label` property instead of the `alt` attribute as we don't have the `img` element inside the <div> element.
Due to our `role` attribute, now screen readers will understand this as being.

## Next up

Work with form elements.
