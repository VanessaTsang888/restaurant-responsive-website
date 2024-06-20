# Lecture 136. Responding to Phones

Show media queries view

Use the Chrome DevTools to inspect the page.
On the top-right click the three dots More options icon.
On the dropdown select 'Show media queries'. This will give us a handy view at the top which will show us what media queries we have set.
When we click on one, it will take us the position of the media query. This way we can see what our page looks like at each of the media queries.

We alrady have media querie at 704px. Now we will create a new media querie of 500px as that is another 200px down.

At 500px we can see the logos no longer fit as they are overlaping each other and the last one is cropped off. How it works sections, the image is now too small and the copy text is too large. Sample Meals, the cards is too small. The Gallery needs to be larger. Pricing section, the plans are too small. CTA, is too small. Set new breakpoint at 550px prox.

550/16 = 34,375 # round off to 34em.
34*16 = 544px

We will have all grids in one col, no longer multiple cols as now we don't have enough space for that anymore.

Reduce the vertical gap.

Test in UI:
I can see the new media querie of 34em at the top.
The images for How It Works section are in wrong order as they were in Z Pattern before.

## Hero Section

Remove extra spacing around Hero header: `.hero` `.section-hero`.

Problem with buttons:
- Too much horizontal space.
- Not enough height for each buttons.
- The styles them are in general.css

Now they fit side by side and also bigger which makes them easier to tap.

Images too small:

Increase the width: `hero-img`. Over-ride css rule with `width: 80%;`.

## As Featured In

The logos are too big: `.logos img`.

## How It Works

Image should be before the copy text so need to switch them over. Each element have their own row.
Manually select the img row and make it the first row by using the enth child func: `:nth-child()` and use number 2 as the parameter as its the second child of the container element we need to target. The number 2 refers to the number of the children of container not the `.stp-img-box` class. 

Fix the spacing between the bottom of image and its copy text below as its too much. They should be closer as they belong together.
Select all image boxes `step-img-box` class and move them down a little using the `transform` property with the `translateY` vertically on the Y-Axis or Y direction. This will move the elements without affecting the elements around it.

## Testimonials

Use the power of CSS Grid to re-layout from 2 to 1 column.

```css
.testimonials {
  grid-template-columns: 1fr;
}
```

## Gallery

Too much spacing between each image and they are all too small so make it 4 by 3 gallery - just 4 cols.

## CTA 

Too small, re-layout in to 1 cols. 

## Summary

This is it for responsive web design and development with HTML and CSS.


