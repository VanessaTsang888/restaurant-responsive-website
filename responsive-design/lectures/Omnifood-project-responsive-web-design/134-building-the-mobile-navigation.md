# 134. Building the Mobile Navigation

For breakpoint below 944px - tablets.

Add new code to index.html file by generate x2 new icons from [ionicons free icon fonts](https://ionic.io/ionicons):

1. the burger menu icon
2. the closed 'X' icon for closed burger menu icon.

Add new code to styles.css using the new class we just written in our html file: `.btn-mobile-nav`. First CSS code block to build the button and style it. Then the second code block to build the x2 icons and style them.

## Icons

Select the close icon and hide it:

styles.css file -> use the same selector again, select the `icon-mobile-nav` element based on the `name` attribute.

```css
.icon-mobile-nav[name='close-outline'] {
  display: none;
}
```

queries.css -> for breakpoint below 944px we show the button.
Work on the `main-nav` element:

- take it out of the flow so its no longer a flex item.
- Make it ocupy the entire screen.
- Then centre content inside of the container.
- content need to layout one after another so change the flex direction using `.main-nav-list` class.
- nav will be hidden by default until user clicks the burger menu icon.
-

This is the correct way to hide an element from screen readers/assistive technology without using `display: none;`:

```css
    /* 3) Hide it from screen readers */
    visibility: hidden;
  }
```

### Now change the menu to close icon:

```css
/* Change open icon to use the close icon when the nav-open element in html shows */
.nav-open .icon-mobile-nav[name='close-outline'] {
  display: block;
}
```

```css
/* Use transition to create animation: Move whole nav to the right  */
transform: translateX(100%);
```
