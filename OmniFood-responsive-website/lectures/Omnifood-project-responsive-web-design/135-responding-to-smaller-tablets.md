# Lecture 135. Responsing to Smaller Tablets

Add another breakpoint at 700px screen width as this is when the design on some sections break or look too crambed.

## index.html

Remove the `nav-open` class.

## queries.css

Convert 700 to em:
700/16 = 43.75 -> round off to: 44em

duration 4:23
I don't think we should comment out the 5 grid css on general.css as its need for desktop devices?

## Section Meals

The Works with any diet list, we want this to span over the 2 cols so it is centered over the 2 cols.

1. html file -> div -> class `diet`. Manipulate in queries.css inside of new media queries of 44em.
2. justify prop is for the horizonal alignment and self is we are setting this now on individual grid item and not on the grid container. Set to centre to layout to center of the 2 grid items. Tested and works as expected.

## How it works section

h2 at 531px width -> too much white-space below it. 

## Pricing Section

Now this look too swoshed in and the two plans need more space.
Note, we need to cover at least 150px. Therefore, design should not break at 579px.
In css we made them only 75% wide which is a problem now. So we need to remove that to set it back to 100%. 
We have a typo issue as class should be pricing-plan not princing-plan. We fix it now. 

Bug I created previously now fixed:
My Pricing plan bug on index.html
Plan complete -> div: i had an extra class I didn't need of:
pricing-plan--starter
Now removed and working and fixed

## Footer section

At 585px, last column disappers from the page which we need to fix.
We need to move the last 3 cols to above the first 2 cols. 