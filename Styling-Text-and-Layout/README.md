# Lesson 2: Styling Text and Layout

Welcome to Lesson 2 of our CSS Basics module! In this lesson, we'll cover how to style text and layout elements on your web pages using CSS.

## Table of Contents

1. [Introduction](#introduction)
2. [Styling Text](#styling-text)
    - [Font Properties](#font-properties)
    - [Text Alignment](#text-alignment)
    - [Text Decoration](#text-decoration)
    - [Text Transformation](#text-transformation)
    - [Text Shadow](#text-shadow)
3. [Styling Layout](#styling-layout)
    - [The Box Model](#the-box-model)
    - [Margin](#margin)
    - [Padding](#padding)
    - [Border](#border)
    - [Width and Height](#width-and-height)
    - [Display](#display)
4. [Examples](#examples)
5. [Resources](#resources)

## Introduction

Styling text and layout is a fundamental aspect of web design. This lesson will teach you how to use CSS to enhance the readability and visual appeal of your web content.

## Styling Text

### Font Properties

CSS provides several properties to style fonts:

- **font-family**: Specifies the font of an element.

  ```css
  p {
    font-family: Arial, sans-serif;
  }
  ```

- **font-size**: Sets the size of the font.

  ```css
  h1 {
    font-size: 24px;
  }
  ```

- **font-weight**: Sets the weight (or boldness) of the font.

  ```css
  strong {
    font-weight: bold;
  }
  ```

- **font-style**: Sets the style of the font (e.g., italic).

  ```css
  em {
    font-style: italic;
  }
  ```

### Text Alignment

- **text-align**: Aligns text horizontally.

  ```css
  h1 {
    text-align: center;
  }
  ```

### Text Decoration

- **text-decoration**: Adds decorations to text (e.g., underline).

  ```css
  a {
    text-decoration: underline;
  }
  ```

### Text Transformation

- **text-transform**: Controls the capitalization of text.

  ```css
  p {
    text-transform: uppercase;
  }
  ```

### Text Shadow

- **text-shadow**: Adds shadow to text.

  ```css
  h1 {
    text-shadow: 2px 2px 5px grey;
  }
  ```

## Styling Layout

### The Box Model

The CSS box model describes the rectangular boxes generated for elements in the document tree and consists of the content, padding, border, and margin areas.

### Margin

- **margin**: Sets the outer space of an element.

  ```css
  .box {
    margin: 20px;
  }
  ```

- **margin-top, margin-right, margin-bottom, margin-left**: Sets the margin for each side of an element.

  ```css
  .box {
    margin-top: 10px;
    margin-right: 15px;
    margin-bottom: 20px;
    margin-left: 25px;
  }
  ```

### Padding

- **padding**: Sets the inner space of an element.

  ```css
  .box {
    padding: 20px;
  }
  ```

- **padding-top, padding-right, padding-bottom, padding-left**: Sets the padding for each side of an element.

  ```css
  .box {
    padding-top: 10px;
    padding-right: 15px;
    padding-bottom: 20px;
    padding-left: 25px;
  }
  ```

### Border

- **border**: Sets the border of an element.

  ```css
  .box {
    border: 1px solid black;
  }
  ```

- **border-width, border-style, border-color**: Sets the width, style, and color of the border.

  ```css
  .box {
    border-width: 2px;
    border-style: dashed;
    border-color: blue;
  }
  ```

### Width and Height

- **width**: Sets the width of an element.

  ```css
  .box {
    width: 100px;
  }
  ```

- **height**: Sets the height of an element.

  ```css
  .box {
    height: 50px;
  }
  ```

### Display

- **display**: Specifies the display behavior (the type of rendering box) of an element.

  ```css
  .inline {
    display: inline;
  }

  .block {
    display: block;
  }

  .none {
    display: none;
  }
  ```

## Examples

Here are some practical examples demonstrating the concepts covered in this lesson:

1. [Basic Text Styling](./examples/text-styling.html)
2. [Box Model Demonstration](./examples/box-model.html)
3. [Layout with Margin, Padding, and Border](./examples/layout.html)

## Resources

- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools - CSS](https://www.w3schools.com/css/)
- [CSS-Tricks](https://css-tricks.com/)
- [freeCodeCamp - Responsive Web Design Certification](https://www.freecodecamp.org/learn/responsive-web-design/)

---

This README provides an overview of Lesson 2: Styling Text and Layout, covering key concepts and CSS properties. For further learning, check out the provided resources and examples.