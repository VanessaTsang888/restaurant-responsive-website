IMPORTANT NOTES:

In general, you should only have one h1 per page, and that h1 should succintly represent the content on that page.

CSS:
Use the class name of the container to style in css.
Using classes in HTML to select everything to layout and style in CSS.

Span <span></span> is a generic text element.
Div <div></div> is just a container without any semanic meaning.

Img's don't auto scale up or down like text do so we have to do this manually:
-> .step-img {
width: 50%;
}

For a scalable page and our code to be cleaner we make use of resuable grid which is more valuable.
Circle to occupy same space as img: using absolute positioning instead of flexbox. Transform circle to its -50% of its own width and -50% of its own height.
Use css property Z Index to move circle behind img.

Summary:
Techniques used:
To center circle with iPhone img we used the

- absolute positioning with the top, left, and the transform: translate()
  To move circle behind img we used the css property 'z-index' with a minus figure.

IMAGES:

Even for images, use flexbox in css file.

SYMBOLS:
<!-- The registered symbol -->
<li class="meal-attribute">NutriScore &reg; 74</li>
