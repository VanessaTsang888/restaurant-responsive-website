# 140. Implementing Smooth Scrolling

Will implement nice animated smooth scrolling rather to desired section so user can see they are still on the same page than a harsh jump.

For Apple mobile devices - iPhones and iPad's only Safari browser is available by default. Therefore, we need to make our smooth scrolling work for Safari.

Use relative path to link-up the main navigations/button and the x2 buttons on Hero section.

Duration 5:05
The anchor for the top of page (not empty link) is missing:
index.html -> header tag: here a need ancher tag or a tag (with href attribute with value of just a hash) around the image tag as this will take user to top of the page as this is a single page website.

## index.html

href attributes: add relative path links.

Use id attribute to give this section tag a unquie name.

```html
<section class="section-cta" id="cta"></section>
```

Then back up to our link, create a page anchor. cta is the id of the section element tag. Move use to that place of the page.

```html
<a href="#cta" class="btn btn--full margin-right-sm">Start Eating Well</a>
```

Once updated the various section tags, update the href attributes within the nav block of code:
`<nav class="main-nav">`

## Safari browser

The smooth scrolling don't work on current version of Safari as I've just test it and failed. This is not good since this is a large page. Therefore we need to use JavaScript to build this functionality.

Smooth scrolling animation
Only select the anchor elements with href attribute.
Add event listener to each of these links as we want to listen for a click event as we want something to happen when user clicks on one of these anchors.

```js
const allLinks = document.querySelectorAll('a:link');
console.log(allLinks);
```

## Close Navigation

On mobile view, when user click on a top level nav, we want the mobile nav to close.
Since the links within the `<nav class="main-nav">` main nav have class name, we can do a check for the class name, if it exists then we just remove the `nav-open` class.
