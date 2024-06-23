# CatPhotoApp

Welcome to the CatPhotoApp repository! This project is a simple web application that displays cat photos, cat-related lists, and includes a form for submitting cat photos. This project covers the basics of HTML from the first three lessons of the Web Development Crash Course.

## Table of Contents

1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Features](#features)
4. [Usage](#usage)
5. [HTML Tag Explanations](#html-tag-explanations)
6. [Contributing](#contributing)

## Introduction

CatPhotoApp is a beginner-friendly project designed to teach the fundamentals of HTML. It includes various HTML elements and attributes, such as headings, paragraphs, links, images, lists, and forms. This project is perfect for those who are new to web development and want to practice their HTML skills.

## Project Structure

The project consists of a single HTML file with the following structure:

- **`<html>`**: The root element of the HTML document.
- **`<head>`**: Contains meta-information and the title of the webpage.
- **`<body>`**: Contains the main content of the webpage.

### Head

```html
<head>
    <meta charset="UTF-8" />
    <title>CatPhotoApp</title>
</head>
```

### Body

```html
<body>
    <main>
        <h1>CatPhotoApp</h1>
        <section>
            <h2>Cat Photos</h2>
            <p>See more <a target="_blank" href="https://github.com/itzmudassir">cat photos</a> in our gallery.</p>
            <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
        </section>
        <section>
            <h2>Cat Lists</h2>
            <h3>Things cats love:</h3>
            <ul>
                <li>cat nip</li>
                <li>laser pointers</li>
                <li>lasagna</li>
            </ul>
            <figure>
                <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
                <figcaption>Cats <em>love</em> lasagna.</figcaption>  
            </figure>
            <h3>Top 3 things cats hate:</h3>
            <ol>
                <li>flea treatment</li>
                <li>thunder</li>
                <li>other cats</li>
            </ol>
            <figure>
                <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">
                <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
            </figure>
        </section>
        <section>
            <h2>Cat Form</h2>
            <form action="https://freecatphotoapp.com/submit-cat-photo">
                <fieldset>
                    <legend>Is your cat an indoor or outdoor cat?</legend>
                    <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
                    <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
                </fieldset>
                <fieldset>
                    <legend>What's your cat's personality?</legend>
                    <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
                    <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
                    <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>
                </fieldset>
                <input type="text" name="catphotourl" placeholder="cat photo URL" required>
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>No Copyright - <a href="https://github.com/itzmudassir">Mudassir Nadeem</a></p>
    </footer>
</body>
```

## Features

- **Cat Photos Section**: Displays a cat photo and provides a link to more cat photos.
- **Cat Lists Section**: Contains unordered and ordered lists of things cats love and hate, along with images and captions.
- **Cat Form Section**: Includes a form for submitting cat photos with radio buttons, checkboxes, and a text input.

## Usage

To use this project, simply clone the repository and open the `index.html` file in your web browser:

```sh
git clone https://github.com/itzmudassir/catphotoapp.git
cd catphotoapp
open index.html
```

## HTML Tag Explanations

Here's a detailed explanation of each HTML tag used in this project:

- **`<!DOCTYPE html>`**: Declares the document type and version of HTML.
- **`<html lang="en">`**: Root element of an HTML document, with the `lang` attribute specifying the language.
- **`<head>`**: Contains meta-information about the document, such as character set and title.
    - **`<meta charset="UTF-8">`**: Sets the character encoding for the document to UTF-8.
    - **`<title>`**: Specifies the title of the webpage, which appears in the browser tab.
- **`<body>`**: Contains the content of the HTML document.
    - **`<main>`**: Represents the main content of the document.
        - **`<h1>`**: Defines the main heading of the webpage.
        - **`<section>`**: Defines a section in the document.
            - **`<h2>`**: Defines a subheading within a section.
            - **`<p>`**: Defines a paragraph of text.
                - **`<a>`**: Defines a hyperlink, with `href` specifying the URL and `target="_blank"` opening the link in a new tab.
            - **`<img>`**: Embeds an image in the webpage, with `src` specifying the image URL and `alt` providing alternative text.
            - **`<h3>`**: Defines a sub-subheading within a section.
            - **`<ul>`**: Defines an unordered (bulleted) list.
                - **`<li>`**: Defines a list item within an unordered or ordered list.
            - **`<figure>`**: Specifies self-contained content, such as an image with an optional caption.
                - **`<figcaption>`**: Provides a caption for the content in the `<figure>` element.
                - **`<em>`**: Emphasizes text, typically rendered in italics.
                - **`<strong>`**: Defines important text, typically rendered in bold.
            - **`<ol>`**: Defines an ordered (numbered) list.
        - **`<form>`**: Defines an HTML form for user input, with `action` specifying the URL where the form data is sent.
            - **`<fieldset>`**: Groups related elements within a form.
                - **`<legend>`**: Provides a caption for the content in the `<fieldset>` element.
                - **`<label>`**: Defines a label for an `<input>` element, improving form accessibility.
                    - **`<input>`**: Defines an input field, with various types such as `radio`, `checkbox`, and `text`.
            - **`<button>`**: Defines a clickable button.
    - **`<footer>`**: Defines the footer of the document or section, typically containing metadata or links.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Open a pull request

Please make sure to update tests as appropriate.