# Lecture 144. Adding Favicon and Meta Description

Now we optimise our page by add a meta desciption to the head tag and add different sizes of favicon also within header tag.

Meta Description

- A short summary of our site content.
- text that will appear of the search results in Google and other search engines.

## Add meta description

index.html
Add meta data to the top of html file.
The summary of our content is the value of the content attribute.

title tag:
Write it better using a dash, colon or bar after Omnifood. Then some other text such as:

Omnifood - Never cook again!
The `&mdash;` is a longer dash punchuashion. Tested and works as expected.

## Favicon

Its the icon on the tab above the browser window.

Its big at 512px and 16kb. This is because we need dmultiple versions of this icon.
Big for Andriod devices.
Desktop devices:
iOS devices:

copy the image file, reduce size to 64px.
`<link rel="icon" href="img/favicon.png" />`
Tested and works as expected.

Home screen - special icon:
iOS: 180px
Andriod: 192px.
Add favicons for all platforms:
Create a brand new file in root of project folder called: manifest.webmanifest
This is file extension used for Andriod to recongnise a different favicons
