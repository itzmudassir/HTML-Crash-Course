# Lesson 3: Creating Forms and Tables

Welcome to Lesson 3 of our HTML Basics module! In this lesson, we'll cover how to create forms and tables in HTML, focusing on the key elements and attributes used to structure and style them.

## Table of Contents

1. [Forms in HTML](#forms-in-html)
    - [Form Elements and Attributes](#form-elements-and-attributes)
    - [Example: Simple Form](#example-simple-form)
2. [Tables in HTML](#tables-in-html)
    - [Table Elements and Attributes](#table-elements-and-attributes)
    - [Example: Simple Table](#example-simple-table)
3. [Resources](#resources)

## Forms in HTML

Forms are used to collect user input in a structured manner. They can include various input elements like text fields, radio buttons, checkboxes, and submit buttons.

### Form Elements and Attributes

- `<form>`: The main container for form elements.
  - **Attributes**:
    - `action`: Specifies the URL where the form data should be sent when submitted.
    - `method`: Specifies the HTTP method to be used when sending form data (`GET` or `POST`).

- `<input>`: Used to create various input fields.
  - **Attributes**:
    - `type`: Specifies the type of input (`text`, `password`, `submit`, `radio`, `checkbox`, etc.).
    - `name`: Specifies the name of the input field, used to identify the data when the form is submitted.
    - `value`: Specifies the initial value of the input field.
    - `placeholder`: Provides a hint to the user about what to enter in the input field.

- `<label>`: Defines a label for an `<input>` element, improving accessibility.

- `<textarea>`: Creates a multi-line text input.

- `<select>`: Creates a dropdown list.
  - **Attributes**:
    - `name`: Specifies the name of the dropdown.
  - `<option>`: Defines an option in the dropdown.

- `<button>`: Creates a clickable button.
  - **Attributes**:
    - `type`: Specifies the type of button (`button`, `submit`, `reset`).

### Example: Simple Form

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Form Example</title>
</head>
<body>
    <form action="/submit-form" method="post">
        <label for="name">Name:</label>
        <input type="text" id="name" name="user_name" placeholder="Enter your name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="user_email" placeholder="Enter your email" required>
        
        <label for="message">Message:</label>
        <textarea id="message" name="user_message" placeholder="Enter your message"></textarea>
        
        <button type="submit">Submit</button>
    </form>
</body>
</html>
```

## Tables in HTML

Tables are used to display tabular data. They consist of rows and columns defined using various HTML elements.

### Table Elements and Attributes

- `<table>`: The main container for table elements.
  - **Attributes**:
    - `border`: Specifies the width of the table border.

- `<tr>`: Defines a row in a table.

- `<th>`: Defines a header cell in a table.
  - **Attributes**:
    - `scope`: Specifies whether the header cell applies to a row, column, or group of rows or columns.

- `<td>`: Defines a standard data cell in a table.

- `<caption>`: Provides a title for the table.

- `<thead>`: Groups header content in a table.

- `<tbody>`: Groups body content in a table.

- `<tfoot>`: Groups footer content in a table.

### Example: Simple Table

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Table Example</title>
</head>
<body>
    <table border="1">
        <caption>Monthly Savings</caption>
        <thead>
            <tr>
                <th>Month</th>
                <th>Savings</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>January</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>February</td>
                <td>$150</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Total</td>
                <td>$250</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
```

## Resources

Here are some additional resources to help you learn more about creating forms and tables in HTML:

- [MDN Web Docs - Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)
- [MDN Web Docs - Tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables)
- [W3Schools - HTML Forms](https://www.w3schools.com/html/html_forms.asp)
- [W3Schools - HTML Tables](https://www.w3schools.com/html/html_tables.asp)

---

This README provides an overview of Lesson 3: Creating Forms and Tables, covering the key elements and attributes used in HTML forms and tables. For further learning, check out the provided resources and examples.