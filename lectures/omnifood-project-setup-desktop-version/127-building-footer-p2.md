# 127. Building the Footer - Part 2

Style and layout the x4 headings which are really just paragraph text but with class name of `footer-heading`. Personally I would of used a heading element which I think I will as one my Quick Wins after I've completed this course.

## Custom grid

Both column 1 and 2 has longer pieces of text. Therefore they need bigger columns. We use CSS Grid Layout to define our custom grid. The value will be in `fr` unit which is equal to 25%.

```css
.grid--footer {
  grid-template-columns: 1.5fr 1.5fr 1fr 1fr 1fr;
}
```

## Separaate footer section from CTA section

Create a suttle line from left to right and above the footer to separate this section from the above CTA section.

```css
.footer {
  padding: 12.8rem 0;
  border-top: 1px solid #eee;
}
```

## Accessibility

For the "Try For FREE" Call To Action, I have added a little `letter-spacing` for better accessibility. Now the letters and not touching each other making the words much easier to read.

Now completed the Desktop version of the Omnifood website application.

## Next up

Make this Desktop version to be responsive / to adapt to smaller screens so when we make the browser window small the elements don't break down.
