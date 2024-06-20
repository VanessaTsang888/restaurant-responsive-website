# Lecture 139. Making the Mobile Navigation Work

On mobile view when user taps the mobile navigation icon which is the hamburger menu then we want to activate the class of `nav-open`.
When do we want to add this class or when do we want the action to happen or where do we need to click in order for something to happen? Its this button here `<button class="btn-mobile-nav">`. Use this class name in our script.js file and select it using the constant keyword so we are declaring a constant.

## script.js

Make mobile navigateion work:

Store our HTML element in the new `btnNavEl` object we are declaring so we can use it later.
List for click event for that btn using the add event listener func and pass-in the click event. There are other events such as hovering or typing some key on the keyboard etc. For second parameter is our own func. Execute the code in body when when user has clicked the btn - the first param. We want to add the class of `nav-open` when its not there, but if its already there then we want to remove it.

We want to work with classes so we use the `classList` property. Toggle will look at the `headerEl` element and if it do have the `nav-open` class then it will not add it. If its already there, it will remove it. otherwise, it will add it.

```js
// Declare new constants and store HTML element in it so we can use those constants later.
const btnNavEl = document.querySelector('.btn-mobile-nav');
const headerEl = document.querySelector('.header');
// When user tap on mobile navigation icon the code in body code block will execute.
btnNavEl.addEventListener('click', function () {
  headerEl.classList.toggle('nav-open');
});
```

### Test in UI

I've tested this functionality in the UI visually and by inspecting the UI and found that it works as expected. However, the focus state is behind the navigation icons so we can't see it working.

## Fix Focus Effect

Now the functionality for the mobile navigation works, we need to fix the focus state/effect as it is currently behind the icon and we can't see it which is a problem for accessibility. We need to ensure the focus state is always stays on top of the navigation - the white background.

```js
/* Accessibility: use the Z-index property
** to ensure the focus state stays on top
** of nav - white background. */
  .btn-mobile-nav {
    display: block;
    z-index: 9999;
  }
```
