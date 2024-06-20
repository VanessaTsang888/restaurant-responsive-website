# Lecture 138. A Short Introduction to JavaScript

Now we write some Javascript code.

## Link up JavaScript file

In HTML file, link up the script.js. To do this we write the script tag.

## Test JavaScript file

In the script.js
This is a very useful way for us to test out some code.

```js
console.log('Hello world!');
```

Test in UI:

Inspect the UI and use the Console tab to test.

- We see the Hello world! plain text which is what we expect.

## Short Intro To JS

Make certain styles only get applied once we actually click on the heading 1. This is dynamic affect we can't do using plain CSS.

In JS we can respond to an event such as a click event. Basically listening for that event on a certain element. We want something to happen when user click on the h1 element. So we can listen for click event on that h1. For this we write the addEventListener func which is a reuseable piece of code.

Test code:

```js
const myName = 'Vanessa Tsang';
const h1 = document.querySelector('.heading-primary');
console.log(myName);
console.log(h1); // <h1 class="heading-primary"></h1>

// Listen for click event on that h1 element as when user clicks h1 execute the code inside of the func body
h1.addEventListener('click', function () {
  // Change the content of h1 to my Vanessa Tsang.
  h1.textContent = myName;
  // Change the CSS
  h1.style.backgroundColor = 'red';
  h1.style.padding = '5rem';
});
```

## Copyright line

Use JavaScript to keep our Copyright line updated for us.

index.html

```html
<p class="copyright">
  Copyright &copy; 2027 by Omnifood, Inc. All rights reserved.
</p>
```
