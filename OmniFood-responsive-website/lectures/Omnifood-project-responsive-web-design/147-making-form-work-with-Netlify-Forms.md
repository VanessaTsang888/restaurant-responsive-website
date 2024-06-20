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
