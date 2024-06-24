# Cafe Menu

Welcome to the Cafe Menu repository! This project is a simple web application that displays a cafe menu with items and prices for coffee and desserts. This project covers the fundamentals of HTML and CSS.

## Table of Contents

1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Features](#features)
4. [Usage](#usage)
5. [HTML Tag Explanations](#html-tag-explanations)
6. [CSS Explanations](#css-explanations)
7. [Contributing](#contributing)

## Introduction

Cafe Menu is a beginner-friendly project designed to teach the basics of HTML and CSS. It includes various HTML elements and attributes, such as headings, paragraphs, links, images, lists, and articles, as well as CSS for styling the webpage.

## Project Structure

The project consists of two files:
- `index.html`: The main HTML file.
- `styles.css`: The CSS file for styling the HTML content.

### HTML Code

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cafe Menu</title>
    <link href="styles.css" rel="stylesheet"/>
  </head>
  <body>
    <div class="menu">
      <main>
        <h1>CAMPER CAFE</h1>
        <p class="established">Est. 2020</p>
        <hr>
        <section>
          <h2>Coffee</h2>
          <img src="https://cdn.freecodecamp.org/curriculum/css-cafe/coffee.jpg" alt="coffee icon"/>
          <article class="item">
            <p class="flavor">French Vanilla</p><p class="price">3.00</p>
          </article>
          <article class="item">
            <p class="flavor">Caramel Macchiato</p><p class="price">3.75</p>
          </article>
          <article class="item">
            <p class="flavor">Pumpkin Spice</p><p class="price">3.50</p>
          </article>
          <article class="item">
            <p class="flavor">Hazelnut</p><p class="price">4.00</p>
          </article>
          <article class="item">
            <p class="flavor">Mocha</p><p class="price">4.50</p>
          </article>
        </section>
        <section>
            <h2>Desserts</h2>
            <img src='https://cdn.freecodecamp.org/curriculum/css-cafe/pie.jpg' alt='pie icon'>
            <article class="item">
                <p class="dessert">Donut</p><p class="price">1.50</p>
              </article>
              <article class="item">
                <p class="dessert">Cherry Pie</p><p class="price">2.75</p>
              </article>
              <article class="item">
                <p class="dessert">Cheesecake</p><p class="price">3.00</p>
              </article>
              <article class="item">
                <p class="dessert">Cinnamon Roll</p><p class="price">2.50</p>
              </article>
            </section>
          </main>
          <hr class="bottom-line">
          <footer>
            <p>
              <a href="https://github.com/itzmudassir/WebDevelopment-Crash-Course" target="_blank">Visit our website</a>
            </p>
            <p class="address">Available on github</p>
          </footer>
        </div>
      </body>
    </html>
```

### CSS Code

```css
body {
    background-image: url(https://png.pngtree.com/thumb_back/fh260/background/20230408/pngtree-coffee-beans-leaves-beans-background-image_2177928.jpg);
    font-family: sans-serif;
    padding: 20px;
}

h1 {
    font-size: 40px;
    margin-top: 0;
    margin-bottom: 15px;
}

h2 {
    font-size: 30px;
}

.established {
    font-style: italic;
}

h1, h2, p {
    text-align: center;
}

.menu {
    width: 80%;
    background-color: burlywood;
    margin-left: auto;
    margin-right: auto;
    padding: 20px;
    max-width: 500px;
    border-radius: 5px;
}

img {
    display: block;
    margin-left: auto;
    margin-right: auto;
}

hr {
    height: 2px;
    background-color: brown;
    border-color: brown;
}

.bottom-line {
    margin-top: 25px;
}

h1, h2 {
    font-family: Impact, serif;
}

.item p {
    display: inline-block;
    margin-top: 5px;
    margin-bottom: 5px;
    font-size: 18px;
}

.flavor, .dessert {
    text-align: left;
    width: 75%;
}

.price {
    text-align: right;
    width: 25%;
}

/* FOOTER */

footer {
    font-size: 14px;
}

.address {
    margin-bottom: 5px;
}

a {
    color: black;
}

a:visited {
    color: black;
}

a:hover {
    color: brown;
}

a:active {
    color: brown;
}
```

## Features

- **Menu Section**: Displays a menu with coffee and dessert items along with their prices.
- **Footer Section**: Contains a link to the GitHub repository and a simple address line.

## Usage

To use this project, simply clone the repository and open the `index.html` file in your web browser:

```sh
git clone https://github.com/itzmudassir/WebDevelopment-Crash-Course.git
cd WebDevelopment-Crash-Course
open index.html
```

## HTML Tag Explanations

Here's a detailed explanation of each HTML tag used in this project:

- **`<!DOCTYPE html>`**: Declares the document type and version of HTML.
- **`<html lang="en">`**: Root element of an HTML document, with the `lang` attribute specifying the language.
- **`<head>`**: Contains meta-information about the document, such as character set, viewport, title, and link to the CSS file.
    - **`<meta charset="utf-8">`**: Sets the character encoding for the document to UTF-8.
    - **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Ensures the webpage is responsive and adjusts to different screen sizes.
    - **`<title>`**: Specifies the title of the webpage, which appears in the browser tab.
    - **`<link href="styles.css" rel="stylesheet">`**: Links the external CSS file for styling the webpage.
- **`<body>`**: Contains the content of the HTML document.
    - **`<div class="menu">`**: A container for the menu content, styled with the `menu` class.
        - **`<main>`**: Represents the main content of the document.
            - **`<h1>`**: Defines the main heading of the webpage.
            - **`<p class="established">`**: Defines a paragraph with the class `established`, styled to be italic.
            - **`<hr>`**: Defines a thematic break (horizontal line).
            - **`<section>`**: Defines a section in the document.
                - **`<h2>`**: Defines a subheading within a section.
                - **`<img>`**: Embeds an image in the webpage, with `src` specifying the image URL and `alt` providing alternative text.
                - **`<article class="item">`**: Defines an article with the class `item`, containing individual menu items.
                    - **`<p class="flavor">`**: Defines a paragraph with the class `flavor`, styled to align left.
                    - **`<p class="price">`**: Defines a paragraph with the class `price`, styled to align right.
            - **`<footer>`**: Defines the footer of the document or section, typically containing metadata or links.
                - **`<a href="https://github.com/itzmudassir/WebDevelopment-Crash-Course" target="_blank">`**: Defines a hyperlink to the GitHub repository, with `target="_blank"` opening the link in a new tab.
                - **`<p class="address">`**: Defines a paragraph with the class `address`.

## CSS Explanations

Here's a detailed explanation of the CSS styles used in this project:

- **`body`**: Sets the background image, font family, and padding for the body of the document.
- **`h1, h2`**: Sets the font size and margins for headings.
- **`.established`**: Styles the established date with italic text.
- **`h1, h2, p`**: Centers the text for headings and paragraphs.
- **`.menu`**:

 Styles the menu container with width, background color, margins, padding, maximum width, and border-radius.
- **`img`**: Centers the images by setting the left and right margins to auto and making them block elements.
- **`hr`**: Styles the horizontal line with height, background color, and border color.
- **`.bottom-line`**: Adds a top margin to the bottom horizontal line.
- **`.item p`**: Styles the paragraphs within items to be inline-block elements with margins and font size.
- **`.flavor, .dessert`**: Aligns the flavor and dessert text to the left and sets their width.
- **`.price`**: Aligns the price text to the right and sets its width.
- **`footer`**: Styles the footer with font size.
- **`.address`**: Adds a bottom margin to the address paragraph.
- **`a`**: Sets the color of the links and styles them differently for visited, hovered, and active states.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or create a pull request.
