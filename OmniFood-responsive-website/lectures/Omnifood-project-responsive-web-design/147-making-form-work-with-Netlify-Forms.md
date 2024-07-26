# Lecture 147. Making the Form Work With Netlify Forms

In the Netlify dashboard, click the Forms main menu:

- Manage forms and submissions without any server-side code or JavaScript.

Netlify can do this for us.

```html
<form name="contact" netlify>
  <p>
    <label>Name <input type="text" name="name" /></label>
  </p>
  <p>
    <label>Email <input type="email" name="email" /></label>
  </p>
  <p>
    <button type="submit">Send</button>
  </p>
</form>
```

Make changes to the form in the index.html file.
Deploy again. I had to add a new attribute to the form tag to get form to work by Netlify:

`data-netlify="true"`
and then I had Deployed my project again using the Netlify website.

## Submission

Within the Netlify website -> Forms menu, scroll down to the 'Active forms' section. Here we can click on my test submission that I just made using my own details.

This form can only take up to 100 submissions per month. After that I will need to pay for the paid plan.

We cannot use this form submission to submit passwords unless I upgrade my Netlify subscription.

### Form validation and digital accessibility

After I completed this lecture I had tested the first two inputs and found that they do not work as expected as they don't include sufficient form validation.

**Email Input**:
During my test on the email input I found that I was able to enter an invalid email address and submit it. Therefore, I had research JavaScript regular expressions or RegEx and how this can be used to valiad an email input. Therefore, I then used RegEx to write and implement my email validation on the email input. To do this I had to include the `addEventListener()` func in my JavaScript code file (instead of using `onclick` func in my html file). As long as I ensure that in my JS file, the email input is properly selected and that I include the `event.preventDefault();` func to ensure a form submission is prevented when user email address is invalid which is defined within the RegEx JavaScript patterns.

**Full name**:
To valiade the Full name input I used the html `pattern` attribute and had written my JavaScript regular expression as the value for this attribute because this adhere's to the [progressive enhancement guidelines](https://www.gov.uk/service-manual/technology/using-progressive-enhancement) that is part of the digital accessibility guidelines.
