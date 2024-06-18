# Lecture 141. Implementing a Sticky Navigation Bar

As soon as the Hero section moves out of the viewport we will get an new event of `IntersectionObserverEntry` -> `intersectionRatio: 0;` and `isIntersecting: false;`. Test for: `isIntersecting: false;`. If so, add sticky nav. `ent` object stands for entery and is the event we just spoke about.

As we enter the Hero section we should get another event (move into viewport) to remove the sticky nav bar when the `isIntersecting` being back to `true`.

## styles.css

Write new style for sticky nav.
The header element in the html file is the entire part that contains the navigation so the entire bar should stay at the top.
Fix the z-index value of entire header - the sticky class.

We used position absolute so its taken out of the flow. This is similar to position fixed so it starts at the top but we need it to start right after the Hero section.

It a little smaller. So give it a fixed height, remove padding top and bottom.

Add box shadow: Horizonally nothing, vertically is 1.2rem, spread of just 3.2rem, black only 3%.

Everyting here is vertically centered thanks to flex-box.

We want sticky nav to start as soon as the Hero section moves out of the viewport / no longer visible. To do this we will use JavaScript - `intersectionObserver()` func.

Use the obs object we just declared to observe HTML element of `section-hero` which is the Hero section.

Fire off an event when the threshold is zero in the viewport.

We get access to an Array of entries, will have an entery per threshold entry.
`ent` stands for entry.

Big jump on page:
as entire header has been taken out of the flow - absolute position. Resolve this problem in styles.css file.

## Remove Sticky Nav

Remove when `isTintersecting: true` which means when user is back on the Hero section.
