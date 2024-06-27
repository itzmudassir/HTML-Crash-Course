# Registration Form Project

This project demonstrates the creation of a registration form using HTML and CSS. Below is a detailed explanation of the HTML and CSS code used in the project.

## HTML Code Explanation

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Registration Form</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form method="post" action='https://register-demo.freecodecamp.org'>
      <fieldset>
        <label for="first-name">Enter Your First Name: <input id="first-name" name="first-name" type="text" required /></label>
        <label for="last-name">Enter Your Last Name: <input id="last-name" name="last-name" type="text" required /></label>
        <label for="email">Enter Your Email: <input id="email" name="email" type="email" required /></label>
        <label for="new-password">Create a New Password: <input id="new-password" name="new-password" type="password" pattern="[a-z0-5]{8,}" required /></label>
      </fieldset>
      <fieldset>
        <legend>Account type (required)</legend>
        <label for="personal-account"><input id="personal-account" type="radio" name="account-type" class="inline" checked /> Personal</label>
        <label for="business-account"><input id="business-account" type="radio" name="account-type" class="inline" /> Business</label>
      </fieldset>
      <fieldset>
        <label for="profile-picture">Upload a profile picture: <input id="profile-picture" type="file" name="file" /></label>
        <label for="age">Input your age (years): <input id="age" type="number" name="age" min="13" max="120" /></label>
        <label for="referrer">How did you hear about us?
          <select id="referrer" name="referrer">
            <option value="">(select one)</option>
            <option value="1">LinkedIn</option>
            <option value="2">Github</option>
            <option value="3">Instagram</option>
            <option value="4">Other</option>
          </select>
        </label>
        <label for="bio">Provide a bio:
          <textarea id="bio" name="bio" rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>
        </label>
      </fieldset>
      <label for="terms-and-conditions">
        <input class="inline" id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" /> I accept the <a href="https://github.com/itzmudassir/WebDevelopment-Crash-Course">terms and conditions</a>
      </label>
      <input type="submit" value="Submit" />
    </form>
    <p class="reference">Made with <span class="heart">❤</span> by <a href="https://www.linkedin.com/in/itzmudassir/">Mudassir</a></p>
  
  </body>
</html>
```

### HTML Tags Explanation

1. `<!DOCTYPE html>`: Declares the document type and version of HTML being used.
2. `<html lang="en">`: The root element of an HTML document, with the language set to English.
3. `<head>`: Contains metadata and links to external resources like stylesheets.
    - `<meta charset="UTF-8">`: Sets the character encoding for the document.
    - `<title>`: Sets the title of the document.
    - `<link rel="stylesheet" href="styles.css" />`: Links to an external CSS file for styling.
4. `<body>`: Contains the content of the document.
    - `<h1>`: A heading tag used for the main title.
    - `<p>`: A paragraph tag used for text content.
    - `<form method="post" action='https://register-demo.freecodecamp.org'>`: Defines a form that sends data using the POST method to the specified action URL.
        - `<fieldset>`: Groups related elements in a form.
            - `<label for="first-name">`: A label for the input field with the id "first-name".
            - `<input id="first-name" name="first-name" type="text" required />`: An input field for text, marked as required.
            - Repeat for "last-name", "email", and "new-password" fields with appropriate types and attributes.
        - `<legend>`: Provides a caption for the `<fieldset>`.
        - `<label for="personal-account">`: A label for the radio button with the id "personal-account".
            - `<input id="personal-account" type="radio" name="account-type" class="inline" checked />`: A radio button for selecting "Personal" account type, checked by default.
            - Repeat for "business-account" radio button.
        - `<label for="profile-picture">`: A label for the file input field with the id "profile-picture".
            - `<input id="profile-picture" type="file" name="file" />`: An input field for file uploads.
        - `<label for="age">`: A label for the number input field with the id "age".
            - `<input id="age" type="number" name="age" min="13" max="120" />`: An input field for numbers with a range between 13 and 120.
        - `<label for="referrer">`: A label for the select dropdown with the id "referrer".
            - `<select id="referrer" name="referrer">`: A dropdown menu for selecting options.
                - `<option value="">(select one)</option>`: A default option with no value.
                - Repeat for other options with values "1", "2", "3", and "4".
        - `<label for="bio">`: A label for the textarea with the id "bio".
            - `<textarea id="bio" name="bio" rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>`: A multi-line input field for text with a placeholder.
        - `<label for="terms-and-conditions">`: A label for the checkbox with the id "terms-and-conditions".
            - `<input class="inline" id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" />`: A required checkbox for accepting terms and conditions.
            - `<a href="https://github.com/itzmudassir/WebDevelopment-Crash-Course">terms and conditions</a>`: A hyperlink to the terms and conditions.
        - `<input type="submit" value="Submit" />`: A submit button for the form.
    - `<p class="reference">Made with <span class="heart">❤</span> by <a href="https://www.linkedin.com/in/itzmudassir/">Mudassir</a></p>`: A paragraph with a reference and a hyperlink to Mudassir's LinkedIn profile.

## CSS Code Explanation

```css
body {
    width: 100%;
    height: 100vh;
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
    font-family: Tahoma;
    font-size: 16px;
  }
  
  h1, p {
    margin: 1em auto;
    text-align: center;
  }
  
  form {
    width: 60vw;
    max-width: 500px;
    min-width: 300px;
    margin: 0 auto;
    padding-bottom: 2em;
  }
  
  fieldset {
    border: none;
    padding: 2rem 0;
    border-bottom: 3px solid #3b3b4f;
  }
  
  fieldset:last-of-type {
    border-bottom: none;
  }
  
  label {
    display: block;
    margin: 0.5rem 0;
  }
  
  input,
  textarea,
  select {
    margin: 10px 0 0 0;
    width: 100%;
    min-height: 2em;
    border-radius: 5px;
  }
  
  input, textarea {
    background-color: #0a0a23;
    border: 1px solid #0a0a23;
    color: #ffffff;
  }
  
  .inline {
    width: unset;
    margin: 0 0.5em 0 0;
    vertical-align: middle;
  }
  
  input[type="submit"] {
    display: block;
    width: 60%;
    margin: 1em auto;
    height: 2em;
    font-size: 1.1rem;
    background-color: #3b3b4f;
    border-color: white;
    min-width: 300px;
  }
  
  input[type="file"] {
    padding: 1px 2px;
  }
  
  a {
    color: #dfdfe2
  }  
  
  .reference {
    text-align: center;
    font-size: 0.8em;
    color: white;
    font-family: 'Roboto', sans-serif;
  }

  .reference a {
    color: white;
    text-decoration: none;
  }
  
 

```css
  .reference a:hover {
    color: #f00;
  }
  
  .reference span {
    color: #f00;
  }
```

### CSS Properties Explanation

1. **`body`**: 
    - `width: 100%`: Ensures the body takes up the full width of the viewport.
    - `height: 100vh`: Sets the height of the body to 100% of the viewport height.
    - `margin: 0`: Removes default margin.
    - `background-color: #1b1b32`: Sets the background color to a dark shade.
    - `color: #f5f6f7`: Sets the text color to a light shade.
    - `font-family: Tahoma`: Sets the font family to Tahoma.
    - `font-size: 16px`: Sets the base font size to 16 pixels.

2. **`h1, p`**:
    - `margin: 1em auto`: Centers the elements with a 1em margin on top and bottom.
    - `text-align: center`: Centers the text.

3. **`form`**:
    - `width: 60vw`: Sets the form width to 60% of the viewport width.
    - `max-width: 500px`: Sets a maximum width of 500 pixels.
    - `min-width: 300px`: Sets a minimum width of 300 pixels.
    - `margin: 0 auto`: Centers the form horizontally.
    - `padding-bottom: 2em`: Adds padding to the bottom of the form.

4. **`fieldset`**:
    - `border: none`: Removes the default border.
    - `padding: 2rem 0`: Adds padding on the top and bottom.
    - `border-bottom: 3px solid #3b3b4f`: Adds a bottom border with a dark color.
    - `fieldset:last-of-type { border-bottom: none; }`: Removes the bottom border for the last fieldset.

5. **`label`**:
    - `display: block`: Makes the label a block element.
    - `margin: 0.5rem 0`: Adds margin on the top and bottom.

6. **`input, textarea, select`**:
    - `margin: 10px 0 0 0`: Adds margin to the top.
    - `width: 100%`: Sets the width to 100%.
    - `min-height: 2em`: Sets a minimum height of 2em.
    - `border-radius: 5px`: Rounds the corners with a 5-pixel radius.

7. **`input, textarea`**:
    - `background-color: #0a0a23`: Sets the background color to a dark shade.
    - `border: 1px solid #0a0a23`: Sets the border color to match the background.
    - `color: #ffffff`: Sets the text color to white.

8. **`.inline`**:
    - `width: unset`: Removes any width constraints.
    - `margin: 0 0.5em 0 0`: Adds right margin.
    - `vertical-align: middle`: Aligns the element vertically in the middle.

9. **`input[type="submit"]`**:
    - `display: block`: Makes the element a block element.
    - `width: 60%`: Sets the width to 60%.
    - `margin: 1em auto`: Centers the element with margin.
    - `height: 2em`: Sets a height of 2em.
    - `font-size: 1.1rem`: Sets the font size to 1.1 rem.
    - `background-color: #3b3b4f`: Sets the background color.
    - `border-color: white`: Sets the border color to white.
    - `min-width: 300px`: Sets a minimum width.

10. **`input[type="file"]`**:
    - `padding: 1px 2px`: Adds padding.

11. **`a`**:
    - `color: #dfdfe2`: Sets the link color.

12. **`.reference`**:
    - `text-align: center`: Centers the text.
    - `font-size: 0.8em`: Sets the font size to 0.8em.
    - `color: white`: Sets the text color to white.
    - `font-family: 'Roboto', sans-serif`: Sets the font family to Roboto.

13. **`.reference a`**:
    - `color: white`: Sets the link color to white.
    - `text-decoration: none`: Removes the underline from links.

14. **`.reference a:hover`**:
    - `color: #f00`: Changes the link color to red on hover.

15. **`.reference span`**:
    - `color: #f00`: Sets the span color to red.

## Responsive Design Principles

1. **Fluid Grids**: Use percentages instead of fixed widths for layout elements to make them adapt to different screen sizes.
2. **Flexible Images**: Ensure images scale within their containing elements to avoid overflow and maintain layout integrity.
3. **Media Queries**: Use CSS media queries to apply different styles based on screen size, orientation, and other characteristics.

### Media Queries Example

```css
/* Base styles */
body {
  font-size: 16px;
}

h1 {
  font-size: 2em;
}

p {
  font-size: 1em;
}

/* Media query for screens wider than 600px */
@media (min-width: 600px) {
  body {
    font-size: 18px;
  }

  h1 {
    font-size: 2.5em;
  }

  p {
    font-size: 1.2em;
  }
}

/* Media query for screens wider than 900px */
@media (min-width: 900px) {
  body {
    font-size: 20px;
  }

  h1 {
    font-size: 3em;
  }

  p {
    font-size: 1.4em;
  }
}
```

### Explanation

- **Base styles**: Define the default font sizes for the body, headings, and paragraphs.
- **Media queries**: Adjust the font sizes for larger screens using `@media` rules.

## Summary

This README provides an overview of the registration form project, detailing the HTML and CSS code used, as well as explaining the responsive design principles and media queries to create a user-friendly, adaptable web form.