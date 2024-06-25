# Lesson 4: Semantic HTML

Welcome to Lesson 4 of our HTML Basics module! In this lesson, we'll explore the importance of semantic HTML and learn about common semantic elements.

## Table of Contents

1. [Importance of Semantic HTML](#importance-of-semantic-html)
2. [Common Semantic Elements](#common-semantic-elements)
    - [`<header>`](#header)
    - [`<nav>`](#nav)
    - [`<main>`](#main)
    - [`<article>`](#article)
    - [`<section>`](#section)
    - [`<aside>`](#aside)
    - [`<footer>`](#footer)
    - [`<figure>` and `<figcaption>`](#figure-and-figcaption)
3. [Resources](#resources)

## Importance of Semantic HTML

Semantic HTML refers to using HTML elements that convey the meaning of the content they enclose, rather than just how it looks. This practice is essential for several reasons:

1. **Accessibility**: Semantic elements help screen readers and other assistive technologies understand the structure and meaning of web pages, improving accessibility for users with disabilities.

2. **SEO (Search Engine Optimization)**: Search engines use semantic HTML to better understand the content of a web page, which can improve search engine rankings.

3. **Maintainability**: Semantic HTML makes code more readable and easier to maintain, as the purpose of each element is clear from its name.

4. **Consistency**: Using semantic elements ensures a consistent structure across web pages, which can help with styling and scripting.

## Common Semantic Elements

Semantic elements describe their meaning in a way that both the browser and the developer can understand. Here are some of the most commonly used semantic elements:

### `<header>`

The `<header>` element represents introductory content or a group of navigational links. It usually contains a heading, logo, or author information.

```html
<header>
  <h1>Welcome to My Website</h1>
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

### `<nav>`

The `<nav>` element is used to define a block of navigation links.

```html
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

### `<main>`

The `<main>` element represents the main content of a document. There should only be one `<main>` element per page.

```html
<main>
  <h2>About Us</h2>
  <p>We are a company dedicated to providing the best services.</p>
</main>
```

### `<article>`

The `<article>` element represents a self-contained composition in a document, page, or site, which is intended to be independently distributable or reusable.

```html
<article>
  <h2>Blog Post Title</h2>
  <p>This is the content of the blog post.</p>
</article>
```

### `<section>`

The `<section>` element represents a thematic grouping of content, typically with a heading.

```html
<section>
  <h2>Our Services</h2>
  <p>We offer a variety of services to meet your needs.</p>
</section>
```

### `<aside>`

The `<aside>` element represents a portion of a document whose content is only indirectly related to the document's main content.

```html
<aside>
  <h2>Related Articles</h2>
  <ul>
    <li><a href="#article1">Article 1</a></li>
    <li><a href="#article2">Article 2</a></li>
  </ul>
</aside>
```

### `<footer>`

The `<footer>` element represents a footer for its nearest sectioning content or sectioning root element.

```html
<footer>
  <p>&copy; 2024 My Website. All rights reserved.</p>
</footer>
```

### `<figure>` and `<figcaption>`

The `<figure>` element represents self-contained content, such as illustrations, diagrams, photos, or code listings, and the `<figcaption>` element provides a caption for the `<figure>` element.

```html
<figure>
  <img src="image.jpg" alt="Description of the image">
  <figcaption>This is a caption for the image.</figcaption>
</figure>
```

## Resources

Here are some additional resources to help you learn more about semantic HTML:

- [MDN Web Docs - HTML Elements Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [W3Schools - HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
- [freeCodeCamp - Semantic HTML](https://www.freecodecamp.org/news/semantic-html5-elements/)

---

This README provides an overview of Lesson 4: Semantic HTML, covering the importance of semantic HTML and common semantic elements. For further learning, check out the provided resources and examples.