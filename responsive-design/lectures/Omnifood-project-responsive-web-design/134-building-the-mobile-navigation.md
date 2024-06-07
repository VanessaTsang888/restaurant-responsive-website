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
{
    /* 3) Hide it from screen readers */
    visibility: hidden;
  }
```

## Now change the menu to close icon:

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

## Accessibility

```css
  .main-nav {
    background-color: rgba(255, 255, 255, 0.97);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    /* Use transition to create animation: Move whole nav to the right  */
    transform: translateX(100%);

    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.5s ease-in;

    /* For Accessibility */

    /* 1) Hide it visually */
    opacity: 0;

    /* 2) Make it unaccessible to mouse and keyboard */
    pointer-events: none;

    /* 3) Hide it from screen readers without using `display: none;` rule. */
    visibility: hidden;
  }
```

Only when the `.nav-open` class do exist in our HTML, then the selector does appy.
Select all elements with a name attribute containing the word 'close-outline'.

```css
  /* Change open icon to use the close icon when the nav-open element in html shows */
  .nav-open .icon-mobile-nav[name='close-outline'] {
    display: block;
  }
```

### Test in the UI

Inspect the UI, reduce the screen width to 666px, in the Elements tab -> header tag -> cut the `nav-open` class, hit the Enter key. Now we see the open menu icon and not the close icon. This is because when the mobile nav is open we want to see the close icon and when the mobile nav is hidden, we show the open menu icon. So the opposit
Next lecture we use JavaScript to do this task rather than CSS.

## Anmination on mobile nav

Use transition property and the translateX func to create animation: Move whole nav to the right - horizontally hence we use the x-axis. We want to move it out of the screen completely by exactly its own width -> value of 100% inside of func.

```css
  .main-nav {
    background-color: rgba(255, 255, 255, 0.97);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    /* Create animation */
    transform: translateX(100%);
```

Note: When we position something absolutely, we should always put position relative on the parent element and in our case here the parent is the `.header` in styles.css, the child is `.main-nav` in queries.css
When this is done, and in the UI, we try to scroll vertically, it will not work which is what we expect.

Tested in the UI and found the animation do work as expected.

We could of used the left property to create the animation but the transform property is way more performent and the animation would not be as smooth as it should be.

The transition property:
Value for transition prop: which property we want to animate, the duration, then the type of the animation.
By default the animation is linear but there are others we can choose from i.e. `ease-in` and over 0.5 second.
 `ease-in` means it move fast at the begining then slow down at the end.

```css
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.5s ease-in;
```

Now finished mobile navigation using html and css.