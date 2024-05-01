# 125 Building Call To Action Section - Part3

To style the label, input and select elements we use the class from the form element then the decendant selector:

```css
.cta-form label {
  display: block;
  font-size: 1.6rem;
  font-weight: 500;
  margin-bottom: 1.2rem;
}

.cta-form input,
.cta-form select {
  /* 100% width: Occpy its entire parent */
  width: 100%;
  padding: 1.2rem;
  font-size: 1.8rem;
  /* Inherit font family from partent element */
  font-family: inherit;
  color: inherit;
  border: none;
  background-color: #fdf2e9;
  border-radius: 9px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}
```

Light colour text inside of input element is known as placeholder.
This don't need to be accessible?

```css
.cta-form input::placeholder {
  color: #aaa;
}
```

## When user hover over the btn

When user hover over the btn the styles will chnage.

```css
.btn--form:hover {
  background-color: #fff;
  color: #555;
}
```

## Accessibility

Focuse state on tab. When user use their tab key to navigate through the page of links they should clearly see where they are on that page. This help with accessibility as some user use their assistive technology due to their reduced eyesight.

Change from the default blue inner borader to our own styles using our orange colour:
`outline: none;`

Select all elements, then use the pseudo class of the focus state.

```css
/* Accessibility: on focus state on tab -> assistive technology: user's with reduced eyesight. */
.cta *:focus {
  outline: none;
  box-shadow: 0 0 0 0.8rem rgb(253, 242, 233, 0.5);
}
```

## Checkboxes

Formating and styling checkboxes are more complicated. Therefore, will save that for another time.
