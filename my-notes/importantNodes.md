IMPORTANT NOTES:

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
