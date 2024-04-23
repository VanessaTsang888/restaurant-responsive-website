# 122. Building the Features Part

Build with total of x4 icons -> class name:`feature-icon`

## Icons

[ionicons](https://ionic.io/ionicons)

1. Use the infinite icons for the Never cook again feature because when you have meals from Omnifood, you'll never need to cook again.

`<ion-icon name="infinite-outline"></ion-icon>`

2. use the nutrition icon for Local and organic feature.

`<ion-icon name="nutrition-outline"></ion-icon>`

3. Use the leaf icon for No waste feature.

`<ion-icon name="leaf-outline"></ion-icon>`

4. Use the pause icon for Pause anytime feature.

`<ion-icon name="pause-outline"></ion-icon>`

## Style and layout with CSS

Now we have the content using HTML5, we can use CSS3 to style and layout the features.

### Classes

```css
.feature-icon {
  ...;
}

.feature-title {
  ...;
}

.feature-text {
  ...;
}
```

### Plan details

HTML5: for this we use the <aside> element because this is additional information not the main content. This often used to develop side bar content but it is infact used for additional information as well.

CSS3 Styles and layout:

```css
.plan-details {
  ...;
}
```

Add space below the element:

```css
.grid:not(:last-child) {
  margin-bottom: 9.6rem;
}
```

This pice of content belongs to the Pricing Plans so it needs to be layout just below the Pricing Plan and centred.

```html
<div class="container grid grid--2-cols margin-bottom-md">...</div>
```

File: general.css

```css
/* helper class */
.margin-bottom-md {
  margin-bottom: 4.8rem !important;
}
```

## Summary

This was apply the design rules, the HTML5 and CSS3 from what I learnt before.
