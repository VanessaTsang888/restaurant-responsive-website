# 126. Building the Footer - Part 1

Now building the content for the footer section using HTML5 to markup the content so that they are semantic.

The <footer></footer> element need to be outside of the <main></main> section as the main area of the website is for non repeated content. The header and footer sections we may repeat them on other pages that are part of the overall website.

The <footer> is used to tell the browser that the content within this element belongs to the footer part of the website. This is HTML5 element to make content semantic.

## Omnifood Logo

When user click on logo, they will be taken back to the top of the page. Since it is a link we wrap it within an <a> element or tag.

```html
<a href="#" class="footer-logo">
  <img class="logo" alt="Omnifood logo" src="img/omnifood-logo.png" />
</a>
```

## social icons

Resources:
[Free icon fonts](https://ionic.io/ionicons)

instagram, Facebook, Twitter.

These need to be links. To make them more semantic we wrap them inside unordered list element then list elements.

```html
<ul class="social-links">
  <li>
    <a class="footer-link" href="#"
      ><ion-icon class="social-icon" name="logo-instagram"></ion-icon>
    </a>
  </li>
  <li>
    <a class="footer-link" href="#"
      ><ion-icon class="social-icon" name="logo-facebook"></ion-icon>
    </a>
  </li>
  <li>
    <a class="footer-link" href="#"
      ><ion-icon class="social-icon" name="logo-twitter"></ion-icon>
    </a>
  </li>
</ul>
```

## Copyright text

The Unicode for the copyright symbol is `&copy;`.

```html
<p class="copyright">
  Copyright &copy; 2027 by Omnifood, Inc. All rights reserved.
</p>
```

## Address

In HTML5, there is an Address element we can use to display our address that makes it semantic.

```html
<address class="contacts">
  <p class="address">623 Harrison St., 2nd Floor, San Francisco, CA 94107</p>
  <p>
    <a class="footer-link" href="tel:415-201-6370">415-201-6370</a><br />
    <a class="footer-link" href="mailto:hello@omnifood.com"
      >hello@omnifood.com</a
    >
  </p>
</address>
```

## Account section

We use the nav element as each content will navigate user to a different page.
We use unordered list element with list element as each piece of text are actually a link.
However, since the pages don't exist as yet, we use the hash charactor as the value for the `href` attribute.

```html
<nav class="nav-col">
  <p class="footer-heading">Account</p>
  <ul class="footer-nav">
    <li><a class="footer-link" href="#">Create account</a></li>
    <li><a class="footer-link" href="#">Sign in</a></li>
    <li><a class="footer-link" href="#">iOS app</a></li>
    <li><a class="footer-link" href="#">Android app</a></li>
  </ul>
</nav>
```
