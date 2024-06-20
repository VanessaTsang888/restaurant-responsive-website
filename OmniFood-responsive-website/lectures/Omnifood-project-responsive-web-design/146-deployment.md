# Lecture 146. Deployment to Netlify

Deploy site on live server and share with others.
There are many web hosting providers on the market. [Netlify](https://www.netlify.com/) is a free service for hosting websites.

Sign up with my GitHub:

- Upload project folder and wait for it to deploy.
- Click the link to see deployed site.

Change the URL as it has random words:

- Change this by click on Site Configuration -> Site information -> Change site name: here rename the URL to: omnifood-vanessa-tsang

## Domain Names

Once I have purchased my own personal domain [Hover](https://www.hover.com/), I can navigate to Domain Management and click the 'Add custom domain' button and configure there.

## Performance Test

Again use Lighthouse Chrome extension and run an Performance test as now we have optimised the images.

Results: Performance 69 but lecture have 99.

in the styles.css I have specified the width but not the height.

```css
.gallery-item img {
  display: block;
  width: 100%;
  transition: all 0.4s;
}
```

### https certificate

Netlify has given us site certificate so our site will stay safe forever.
