Responsive Onine Restaurant Website Project:

L100: Section Intro:
Will bring me to an intermediate level CSS Developer.

L0101: The 7 Steps to a Great Website:
Thinking and planning: The 7 Steps: part of the development process.

1. Define
2. Plan
3. Sketch & layout
4. Design and Build
5. Test and Optimise
6. Launch
7. Maintain and Update.

Defining the Project:

1. Define who the website is for? Who are the users?
2. What is the website is for? What is the main goal of the site? Is it to provide info, i.e. menu's? To sell some product? To allow users to book a table at a restaurant?
   Both the business and user goals of your website project (UX Design). Example, Chinese restaurant: business goal: to provide customer with their latest menu's, restuarnt location and contact details. User goal: to search and read restaurant menu with prices and contact details and to provide feedback on their experience.
3. Define a target audience. Normally this come from your client. Example, anyone who wants to eat authenic Chinese meals, i.e. mainland Chinese students as they have money to spend.

- competition research, userpersonas etc -> marketing/UX Design.

Planning The Project:
Thinking about our website.
Plan and gather site content: copy, images, videos etc i.e. online image libraries.
Bigger site needs a sitemap: what pages the site needs, and how they are related to one another (content hierarchy).
Plan the sections each page should have in order to convey the content's message and in which order. It should be the content that guides the project and the design of the site, NOT the other way round.
website personality.

Sketch:
What components/layouts to use? Sketch on paper or use Figma to produce the wireframes. Important createive process.
This is iterative process so its not set in stone yet so need to make it perfect.

Design and Build Website:
Take the plan, layout and components to develop the site using HTML, CSS and JS based on the site personality. it's common that customer will have some kind of branding in place, i.e. logo, colors etc.

Test and Optimise:

1. ensoure site works well in all major browsers: chrome, Firefox, Safari, Edge, amy be the old IE.
2. Test site on mobile devices. Optise all images - give them correct dimensins in pixiles and compress them down for performance.
3. Fix simple accessibility problems, e.g. color contrast issues. Run a performance test in our Chrome developer tools called Lighthouse.
4. Think about organic SEO.

Launch:
Share my master piece with the world. Upload to a hosting platform and we'll use Netlify -> the free plan. Buy a domain name so users and find my site. Create one that is memorable for the users and easy to write and one that represents the company or the brand.

Maintain and Update:
The site content will need updating over time e.g. menu's and contact details etc.
This can get recurring revenu by creating a monthly contract with customer. Install some kind of analytics software e.g. Google Analytics -> use sates to adapt site, do some fine tuning, make it better and better over time. A blog site needs to be kept up to date all the time but its good way to keep users coming back to your site and good for SEO when you use it with the right content.

L102: Defining and Planning the Project:
OmniFood is a fictional startup. They use AI to create and deliver custom healthy meal plans. They new modern clean website that make them look trustworthy and professional company.
We have all the content for the site.

Define WHO the site is for:

- For a client - OmniFood: read the doc provided from client - About Omnifood.

Define WHAT the website is for:

- Business goal: selling monthly food subscription.
- User goal: eating well effortlessly, without speding a lot of time and moeny.

Define Target Audience:

- targeted at ppl who are into tech.
- ppl who are interested in their health
- ppl who are busy
- ppl who have well paid job due to monthly subscription.
  So busy ppl who likes tech, interest in a healthy diet and have a well-paying job.

Planing The Project:
No need to for a sitemap since its just one page website - landing page.
Comsure well-bing.
The content will guide the design - layout and component.

L103: Sketching Initial Layout Ideas:

- Logo + navigation
- Hero
- Featured in
- How it works
- Meals (and list of diets)
- Testimonials + gallery
- Pricing + features
- CTA
- Footer

Hero:
The design and layout must follow the content.
Use a common form of Hero section.

Feature In Section:
Z-pattern. Some logos next to each other.

How it works section:
Steps from 1 - 3.

Meals section:
Will have 2 meals.

Testimonials + gallery section:
2 by 2 grid. Two components side by side.

Do sketches by hand first. Then may be using Figma. This is the itial plan in how we will build the layout.

L04: First Design and Development Steps (Step 4):
Write first lines of code. Quick setup.
My first design decisions and setting up first design systems.

L105: Responsive Design Principles:
The basics of responsive web design and start right at the begining.
A set of best practices and of techniques that we use in our regular CSS.
Site to work for to all screen sizes even if we initially build and test for big screens.

Responsive Web Design is a technique to make a webpage adjust its layout and visual style to any possible screen size (incl. window or viewport size of browser). Works well on all
devices including desktops, laptop, tablets and smart phones. This site will be easily consumable on all of these devices.

Four Big Ingredients for RWD:

1. Fluid Layouts
2. Responsive Units
3. Flexible Images
4. Media Queries

Fluid Layouts:

- FlexBox and CSS Grid (fluid by default): to allow webpages to adapt to the current viewport width (or even height).
- To create fluid layouts, Use % (or vh / vw) unit instead of px for elements that should adapt to viewport (usually layout).
- Use max-width instead of width.

Responsive Units:

- Use rem unit instead of px for most lenghths.
- To make it easy to scale the entire layout down (or up) automatically.
- Helpful trick: setting 1rem to 10px for easy calculations.

Flexible Images:

- By default, images don't scale automatically as we change the viewport, so we need to fix that.
- Always use % for image dimensions, together with the max-width property.

Media Queries:

- Allows devs to create different versions of site for different types of devices, since differenct types of devices have a different width.
- Bring responsive sites to life!
- To change CSS styles on certain viewport widths (called breakpoints).

Start all these at the beginning.

Desktop-First VS. Mobile-First Development:
Desktop-First Development:

- Start writing CSS for the desktop: large screen.
- Then, media queries shrink design to smaller screens.

Mobile-First Development:
The other way round.

L106: How rem and max-width Work:
How rem and max-width properties Work.
/_ max-width: f the container width is less than the specified max width, then the width of the elementwill be 100% of the container element width. _/

rem is the root elements font-size. The root of the document is the HTML element (the parent element of all the others). 1 rem is equal to the default browser font-size, which is 16px.
1 rem = 16px -> 16 x 50rem = 800px

2rem is 32 px.

By changing the font size we change the entire layout. Set html to 10px so its esay to do the calculations so 1rem will be 10px. But this will cause usability issues for users
whom need to increase or even to decrease the font size of their browsers. To aviod this we not set font-size to fixed value like 10px but instead to a % of the default font-size
of the browser. Used widely in the css developer community. Now we never use px and always use rem.

L107: Building the Hero - Part 1:
Hero image on right side, content - headline on left side. This is like the hearder section.
Split Editor Right: top-right of VSCode

We use muliple section elements which then becomes something bigger. The article element is more self contained.
A div element is just a box without any semantic meaning at all.
Everything will always be selected using classes not id's etc as this will give our css code more consistency.
For button element, we use an Anchor element - a link.
A button should only be used for actions not going to another page. Come up with mirco copy. Subscribe to the OmniFood subscription.
Micro copy: Start Eating Well Now.
This is more compelling than sign UP Now.
Button 02: get additional info -> Learn More. html entity -> &darr; -> down arrow: https://dev.w3.org/html5/html-author/charref
Now make the image flexible, so start styling the layout using css grid.
Even if we use Flexbox instead of CSS Grid we still need some kind of container element for these 2 boxes - the image box and the text box. So the Grid container
could be the section-hero from the section element. But this mean we can't create a fixed size container so we create new div element with class of hero. So this hero
will be our css container:

.hero {
display: grid;
grid-template-columns: 1fr 1fr;
}

Now make image flexible:
<img />
Don't forget the alt text attribute for accessibility (users who can't see images) and for SEO.
The parent element for <img />
is the div with class of hero-img-box. The image will have half the width of the container.
We have a div called hero is to give it a fixed width.

L108: Building the Hero - Part 2:
More visual styles to Hero section.
Using rem (not pixels) unit to resize everything on page such as the font size, but for letter-spacing use px:
letter-spacing: -0.5px;

.hero
Since we are using a Grid Container we can align-items: center for the h1 and paragraph elements.

The visual style of this section -> spacing & colors:
xxx
6:13
Tint and shade generator: https://maketintsandshades.com
https://maketintsandshades.com/#e67e22
#fae5d3 -> use this shade for the entire background for Hero section.
with background-color always need alot of padding top & bottom

To style the buttons, we need to style button link and button visited:
.btn:link, .btn:visited {...}
-> need padding - inline object needs inline block: padding: 1.6rem;
-> For white boarder on secondary btn, use border inside Trick: box-shadow: inset 0 0 0 3px #fff;
-> For the Primary btn, use a simple css animation so it don't jump from one colour to another.
We want to animate both the background-color and the color.
New css property to do smple animation:  
 transition: background-color 1s;
We always put transition on original state.

Fix the space between the 2 btn's using a Helper Class: margin-right-sm

109: Building the Hero - P3:
Finish building Hero Section.

- Select new type face using Goodle fonts: https://fonts.google.com/
- Rubik: https://fonts.google.com/specimen/Rubik?query=rub

components.
last-child -> decendants -> the last img don't need to be overlap so don't need margin-right: -1.6rem -> so write new css class for this: delivered-img img:last-child
Frame around all img same color as the bg.
Check the Contrast Rasio is correct: coolors.co -> contrast checker: past color in and bg color = very poor contrast so use the darker orange - its bold text.

Need vertical spaces between the btn component and the component that hold the imgs which is the div with class of: delivered-meals

imgs: boarder to give them some visible space. Just a small detail but makes it look more designed.
text: make it darker orange -> inlin element.

110 Building The Header:
Put logo and left and nav on right. Not in the fixed width Hero section container but outside it.

<header class="header">
xxxx
</header>

The nav element is used for major navigation of our page. Name it main-nav as will need nav for footer later.

<nav class="main-nav"></nav>

Another New HTML5 semanic element is the main element for the main area of a webpage.
Not include content repeated across multiple pages i.e. <header>
Don't need to give it any class as we don't need to style it. For digital accessibility - screen readers.

Work on layout and visual styles of logo. Use flexbox where header is flex container.

Later will use media queries to make it even more responsive.

111: Building the Navigation:
It is semanic to put links or list items inside of unordered list element <ul></ul>

Use a hash # in the ancher tag until I know where the link should point to. Will link to different section of the page.
Use flexbox:

.main-nav-list {
list-style: none;
display: flex;
gap: 3.2rem;
}

Style the anchors themselves using: main-nav-link calss:

<li><a class="main-nav-link" href="#">Section 1</a></li>

Call To Action btn:
Use 'last child sudo class' to style CTA btn:
It's common to have a CTA in the nav. So we need another class on the last anchor tag <a></a> so we can style this separately.
-> nav-cta
-> border-radius for CTA should always be in px not rem as we don't want them to change.

112: Setting Up a Reusable Grid:

Using the CSS Grid concept to create columns for our How It Works Section:
-> .grid {
display: grid;
gap: 9.6rem
}

-> inside of our view port will be the container to center our content:
.container {
max-width: 120rem;
margin: 0 auto;
}

Check the box model via the Chrome DevTools -> Element -> Styles.

      <section class="section-how">
        <div class="container grid grid--2-cols">

From now on we will use this grid under GENERAL REUSABLE COMPONENTS:

113 Building the How-it-Works Section - P1:
We will use the Z-Pattern design.

HTML: arrange the content in z-pattern.

114 Building the How-it-Works Section - P2:

Continue to use our resuable grid for this section to layout and style content.
create another grid setting on top of this one:
-> .grid { ... }

Too much white space between text and img so we will create a circle in the background but not in the HTML code as we don't polute our HTML with visual things. Instead we use sudo-element.
-> insert a child element inside a parent element.
sudo-element cannot be added to images, as in html themselves we not allowed to add child elements to images.

To make it circle shape use: border-radius: 50%;
To put circle behind img: use css property 'Z Index'.

115 Building the Featured-In Section:
OmniFood has been featured in these 5 big publications:
Logos layout side-by-side, all with same height with heading on top.
Make img from full color to gray:

.logos img {
height: 3.2rem;
filter: brightness(0);
opacity: 65%;
}

116 Building the Meal Section - P1:
Meals + Diets Section.
Cards.
Use the grid class that has 3 cols -> reusable grid we already created:

<div class="container grid grid--3-cols">

                <!-- Fire icon created by https://ionic.io/ionicons -->
                <li class="meal-attribute"><ion-icon name="flame-outline"></ion-icon>650 Calories</li>

Put this in the head tag:

<script nomodule src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.js"></script>

117 Building the Meal Section - P2:
Use the meal-attribute in html and the flexbox in css to vertically align the icons with the text.

Design/ Style the card:
CSS: .meal | .meal-content | .tag | .meal-title | meal-attributes | .meal-attribute | .meal-icon | .meal-img

Create the second card based on the first card:

117 Building the Meal Section - P2:
Create the Diet list within the sample meals.

- remove the bullet within the list item
- format and style the check icon

See all recipes link:

- remove the auto underline with text-decoration: none;
  and then use border-bottom and padding-bottom :

.link:link,
.link:visited {
display: inline-block;
color: #e67e22;
text-decoration: none;
/_ will take the current text color as the border-bottom. Since using padding, need to set to inline-block. _/
border-bottom: 1px solid currentColor;
padding-bottom: 2px;
}

The currentColor keyword will take the current text color as the border-bottom. Since using padding, need to set to inline-block.

.link:hover,
.link:active {
color: #cf711f;
/_ The border-bottom of 1px will disapear on hover _/
border-bottom: 1px solid transparent;
}

Set center-text on container class so the below two classes will inherit it:

<section class="section-meals">
<div class="container center-text">
<span class="subheading">Sample Meals</span>
<h2 class="heading-secondary">

We can use hover on something thats not a link;

Move img up on hover - the y-axis. First figure is for horizonal(x) movement, second is for vertical(y) movement.

.meal:hover {
transform: translateY(-1.2rem);
}

and...
use transition in the original state to move card up:

.meal {
box-shadow: 0 2.4rem 4.8rem rgba(0, 0, 0, 0.085);
border-radius: 11px;
/_ padding: 4.8rem; _/
overflow: hidden;
transition: all 0.4s;
}
