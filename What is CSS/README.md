# What is CSS?

Cascading Style Sheets (CSS) is a style sheet language used to describe the presentation of a document written in HTML or XML. CSS defines how elements should be rendered on screen, on paper, in speech, or on other media.

## Table of Contents

1. [Introduction](#introduction)
2. [Why Use CSS?](#why-use-css)
3. [How CSS Works](#how-css-works)
4. [CSS Syntax](#css-syntax)
5. [Types of CSS](#types-of-css)
6. [Selectors](#selectors)
7. [Properties](#properties)
8. [Units](#units)
9. [Advanced Topics](#advanced-topics)
10. [Resources](#resources)

## Introduction

CSS is one of the core technologies for building web pages, alongside HTML and JavaScript. CSS is used to control the layout of multiple web pages all at once. External stylesheets are stored in CSS files.

## Why Use CSS?

CSS allows you to:

- **Separate content from presentation:** This makes it easier to maintain and update your web pages.
- **Improve loading times:** CSS can reduce the amount of code in your HTML files, leading to faster page loading.
- **Create responsive designs:** CSS provides tools like media queries to create designs that adapt to different screen sizes and devices.
- **Enhance user experience:** CSS can be used to create visually appealing web pages, improving user engagement.

## How CSS Works

CSS works by associating rules with HTML elements. These rules specify how the content of the elements should be displayed. A CSS rule consists of a selector and a declaration block.

- **Selector:** Indicates which HTML element the rule applies to.
- **Declaration block:** Contains one or more declarations separated by semicolons. Each declaration includes a property and a value.

## CSS Syntax

A CSS rule-set consists of a selector and a declaration block:

```css
selector {
  property: value;
}
```

Example:

```css
p {
  color: red;
  font-size: 16px;
}
```

This rule applies to all `<p>` elements, making their text red and setting the font size to 16 pixels.

## Types of CSS

There are three ways to apply CSS to HTML:

1. **Inline CSS:** Uses the `style` attribute inside HTML elements.

   ```html
   <h1 style="color: blue;">Hello World</h1>
   ```

2. **Internal CSS:** Defined within the `<style>` element inside the `<head>` section of an HTML document.

   ```html
   <head>
     <style>
       h1 {
         color: blue;
       }
     </style>
   </head>
   ```

3. **External CSS:** Linked to an HTML document using the `<link>` element.

   ```html
   <head>
     <link rel="stylesheet" type="text/css" href="styles.css">
   </head>
   ```

## Selectors

Selectors are used to target HTML elements. Here are some common types:

- **Element Selector:** Targets all elements of a given type.

  ```css
  p {
    color: blue;
  }
  ```

- **Class Selector:** Targets elements with a specific class attribute.

  ```css
  .my-class {
    color: green;
  }
  ```

- **ID Selector:** Targets an element with a specific ID attribute.

  ```css
  #my-id {
    color: red;
  }
  ```

- **Attribute Selector:** Targets elements with a specific attribute.

  ```css
  [type="text"] {
    border: 1px solid black;
  }
  ```

- **Pseudo-class Selector:** Targets elements in a specific state.

  ```css
  a:hover {
    color: purple;
  }
  ```

## Properties

CSS properties are used to style HTML elements. Some common properties include:

- **Color:** Sets the color of text.

  ```css
  color: blue;
  ```

- **Font-size:** Sets the size of text.

  ```css
  font-size: 16px;
  ```

- **Margin:** Sets the outer spacing of elements.

  ```css
  margin: 10px;
  ```

- **Padding:** Sets the inner spacing of elements.

  ```css
  padding: 10px;
  ```

- **Border:** Sets the border around elements.

  ```css
  border: 1px solid black;
  ```

## Units

CSS supports various units to specify lengths. Some common units include:

- **px (pixels):** Fixed unit.

  ```css
  font-size: 16px;
  ```

- **em:** Relative to the font-size of the element.

  ```css
  padding: 1em;
  ```

- **rem:** Relative to the font-size of the root element.

  ```css
  margin: 1rem;
  ```

- **% (percentage):** Relative to the parent element.

  ```css
  width: 50%;
  ```

## Advanced Topics

- **Flexbox:** A layout model for arranging items in a one-dimensional space.

  ```css
  display: flex;
  ```

- **Grid:** A layout model for arranging items in a two-dimensional space.

  ```css
  display: grid;
  ```

- **Animations:** Allows you to create animations.

  ```css
  @keyframes my-animation {
    from {opacity: 0;}
    to {opacity: 1;}
  }
  ```

- **Media Queries:** Allows you to apply styles based on the viewport size.

  ```css
  @media (max-width: 600px) {
    body {
      background-color: lightblue;
    }
  }
  ```

## Resources

Here are some additional resources to help you learn CSS:

- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools - CSS](https://www.w3schools.com/css/)
- [CSS-Tricks](https://css-tricks.com/)
- [freeCodeCamp - Responsive Web Design Certification](https://www.freecodecamp.org/learn/responsive-web-design/)
