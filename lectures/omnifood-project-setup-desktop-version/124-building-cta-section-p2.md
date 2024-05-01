# 124. Building the Call-To-Action Section - Part 2

Working with form elements for the first time on this project.

## Styling text

Intergrate the colour of heading 2 (h2 -> dark brown) into the orange colour background.

[Make Tint Sand Shades](https://maketintsandshades.com/#e67e22)

Choose/click the dark brown for the h2: #2e1907

File: style.css:

The background is the `.cta` class and the h2 text is the `.cta-text-box` and the `.cta .heading-secondary`.

```css
.cta {
  background-image: linear-gradient(to right bottom, #eb984e, #e67e22);
  /* Fix the img overlapping the cta element. */
  overflow: hidden;

  .cta .heading-secondary {
    color: #45260a;
    margin-bottom: 3.2rem;
  }

  .cta-text {
    font-size: 1.8rem;
    line-height: 1.8;
  }
}
```

To check the accessibility on colour contrast is valid, use the [Color Contrast Checker](https://coolors.co/contrast-checker/45260a-eb984e) tool.

## Building the form

code the form elements using HTML5 and CSS3.
The form element is just box or container for the input elements.

Full Name input: for the type attribute, use the text value which is the most common one.
To send the user's data we need the action attribute with value of URL where the data should be sent to on the serverside.

### Input's

The type attribute -> values:

Full Name: `type="text"`
Email address: `type="email"`
Please choose one option: `value="friends"`
Sign up now: `????`

By default the label and input elements are inline elements so they sit side by side.

### Labels

When we click on them, the associated input field will beome actived. I feel thi is good for accessibility. We do this, inside of the input element, we writing an `id` with value of whatever we wish to call the input.

### for attribute

Use to link the lable to the input and write `for` attribute and use the same value as per the value for the id attribute.

### option element

First option has empty value as user can't submit form with that option still selected.

### required attribute

Add this to any input and select element that requires user to complete. No value is needed.

For each input, the select and the button, wrap in side a set of <div> to make them block level elements. Then format th elements into a nice 2 by 2 grid.
