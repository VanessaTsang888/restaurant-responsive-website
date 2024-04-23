# 121. Building the Pricing Section - Part 2

Continue from previous lecture to finish the Pricing section.

Each of the pricing plans are too wide. Need to adjust the grid cells within the 2 column grid.

I found a typo on the class of `princing-plan` as the word 'princing' should have the letter 'n' in it. Should be like this `pricing-plan`.

Align a grid item inside of a rid cell because the plan Starter is aligned left and we need it to align right to remove the large space between the two plans. Therefore, we use the justify items property.

```css
/* Align the starter plan to the right to remove the space to the right. */
.princing-plan--starter {
  justify-self: end;
}
```

## Visual hierarchy

At the moment the two pricing tables look the same but we want user to select the Complete plan as that one make the company more money. Therefore, we can state that one is best value to make that one stand out more. To do this we use CSS to highlight this point.

### Add ribbon flash to Complete Plan

Location: top-right corner.
Code - CSS:

- Build the content, layout (i.e. on an angle) and styles.
- Use pseudo element.
- To layout the ribbon on an angle we use percentages as the unit for flexible layout.
- inspect the UI and change the css code temporary to get the values right before commiting the change on the styles.css file.
- To cut-off the end parts we use the `overflow` property with value of `hide` but on the parent element which is `princing-plan--complete`:

```css
.princing-plan--complete {
  overflow: hidden;
}
```
