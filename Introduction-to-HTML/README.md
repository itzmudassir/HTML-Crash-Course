# Lesson 1: Introduction to HTML

Welcome to Lesson 1 of our HTML Basics module! In this lesson, we'll introduce HTML and explain the basic structure of an HTML document.

## Table of Contents

1. [What is HTML?](#what-is-html)
2. [Basic Structure of an HTML Document](#basic-structure-of-an-html-document)
3. [Examples](#examples)
4. [Resources](#resources)

## What is HTML?

HTML (HyperText Markup Language) is the standard language for creating web pages. It describes the structure of a web page and consists of a series of elements that tell the browser how to display the content.

### Key Points about HTML

- **Markup Language**: HTML is not a programming language but a markup language used to structure content on the web.
- **Elements and Tags**: HTML uses elements, represented by tags, to define different parts of a webpage.
- **Attributes**: HTML elements can have attributes that provide additional information about the element.
- **Browsers**: Web browsers read HTML files and render them into visible or audible web pages.

## Basic Structure of an HTML Document

An HTML document has a defined structure, which includes a doctype declaration, HTML elements, and nested elements to structure content.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
    </header>
    <main>
        <p>This is a paragraph of text on my website.</p>
    </main>
    <footer>
        <p>© 2024 My Website</p>
    </footer>
</body>
</html>
```

### Explanation of the Basic Structure

- `<!DOCTYPE html>`: This declaration defines the document type and version of HTML. For HTML5, it is simply `<!DOCTYPE html>`.

- `<html lang="en">`: The `<html>` element is the root element of an HTML page, and the `lang` attribute sets the language of the document.

- `<head>`: The `<head>` element contains meta-information about the document, such as its title and character set.

  - `<meta charset="UTF-8">`: This element specifies the character encoding for the document.

  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: This element ensures proper rendering and touch zooming on mobile devices.

  - `<title>Document Title</title>`: This element sets the title of the document, which appears in the browser tab.

- `<body>`: The `<body>` element contains the content of the HTML document, such as text, images, links, etc.

  - `<header>`: Typically contains introductory content or navigational links.

  - `<h1>`: Represents a top-level heading.

  - `<main>`: Represents the main content of the document.

  - `<p>`: Represents a paragraph of text.

  - `<footer>`: Contains footer information, such as contact info or copyright notice.

## Examples

Here are some practical examples demonstrating the basic structure of an HTML document:

1. [Simple HTML Document](./examples/simple-html.html)
2. [HTML Document with Basic Elements](./examples/basic-elements.html)

## Resources

- [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [W3Schools - HTML](https://www.w3schools.com/html/)
- [freeCodeCamp - Responsive Web Design Certification](https://www.freecodecamp.org/learn/responsive-web-design/)

---

This README provides an overview of Lesson 1: Introduction to HTML, covering what HTML is and the basic structure of an HTML document. For further learning, check out the provided resources and examples.