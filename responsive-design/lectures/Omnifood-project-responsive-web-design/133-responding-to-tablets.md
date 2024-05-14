# Lecutre 133 Responding to Tablets

Test to see where the design breaks. Our design breaks around 944px so this is where we put our breakpoint.

Adding another breakpoint and another media query to respond to tablets.

Media query should work over a range of at least 200 or 300 pixels. We don't fix every design problem that appears as we scale down the page. So now we go down 300px to 900px and analyse what our design looks like and if we need to fix something here.

## Add new media query

Add new media query at 940px as any less than that the design breaks - the H1 on hero section.

### Add media query at below 944px

Scale down the value of 1rem even more to make the entire design a bit smaller. We make 1rem to equal to 8 pixels. We want our font size to be 50% as our target is 8px.

8px / 16px = 0.5 = 50%

```css
@media (max-width: 59em) {
  html {
    /* 8px / 16px = 0.5 = 50% */
    font-size: 50%;
  }
```

Now we need it go one column as the images are too small now.
Selectors to change:

`.hero` `.hero-text-box` `.hero-img` `.hero-img` `.delivered-meals`

Test at 748px to check the design work at that breakpoint. Also test that it works at least across 200px.

Reduce the size of logos in the As Featured In section.

Sample Meals:

CSS Grid:
Too much white space within each card. Reduce the white space to be more inline with the rest of the content. To fix this use the `.meal-content` class that is located in the styles.css

Testimonials:

Need to relayout the gallery to give the testimonials more room.
Change gallery grid: 6 cols x 2 rows -> wider.

### Add media query at below 807px

As this is when the design breaks again - the H1 go on four lines with a widow at the ends.

Price plans:
increase the line height of the text.

CTA Section:

- relayout the input fields as they are too short at the moment.
- To do this change the CSS grid values.
- Sign up button: need more space at the top and bottom so the button text is more legible
