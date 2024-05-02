# 129. How media queries work

This is for Desktop First but there is also Mobile First stategy as well.

Maximum width at which media query still applies:

```css
@media (max-width: 600);
```

-> "Is width <= 600px?""
-> Example, at a viewport width of 400px, CSS in both media queries applies.

```css
@media (max-width: 1200px);
```

-> "Is width <= 1200px?".

Code outside of any media query.

## Breakpoints

This is the width we should use in our design as there are many different ways we can select these breakpoints. We can choose the value of the width. Examples:

```css
@media (max-width: 600px) {
  ...;
}
```

## The code

Install the Chrome DevTools browser extension. Inspect the UI. Pull the browser window in and out from the right to see the media queries work.

At 600px and less (<=), we see both the section hero change from the plain orange background to have the dashed blue border around it.

At greater than 1200px, we don't see the section hero to have the orange background as this colour background is only for 1200px and less (<=)

```css
/* Media queries - desktop */

@media (max-width: 600px) {
  .section-hero {
    border: 20px dashed blue;
    background-color: blue;
  }
}

@media (max-width: 1200px) {
  .section-hero {
    background-color: orangered;
  }
}
```

## Next up

130. How to Select Breakpoints:

How do we know which value we should choose for the width and how many media queries we should write?
