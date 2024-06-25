# Lesson 3: Flexbox and Grid

Welcome to Lesson 3 of our CSS Basics module! In this lesson, we'll explore two powerful CSS layout techniques: Flexbox and Grid.

## Table of Contents

1. [Introduction to Flexbox](#introduction-to-flexbox)
    - [What is Flexbox?](#what-is-flexbox)
    - [Basic Flexbox Properties](#basic-flexbox-properties)
    - [Flexbox Examples](#flexbox-examples)
2. [Introduction to Grid](#introduction-to-grid)
    - [What is CSS Grid?](#what-is-css-grid)
    - [Basic Grid Properties](#basic-grid-properties)
    - [Grid Examples](#grid-examples)
3. [Resources](#resources)

## Introduction to Flexbox

### What is Flexbox?

Flexbox, or the Flexible Box Layout Module, is a CSS layout model that allows you to design a flexible and efficient layout structure. Flexbox provides an easy and clean way to arrange items within a container, even when their size is unknown or dynamic.

### Basic Flexbox Properties

- **`display: flex;`**: This property is applied to a container element to activate flexbox layout for its children.

```css
.container {
  display: flex;
}
```

- **`flex-direction`**: This property defines the direction of the flex items.

```css
.container {
  flex-direction: row; /* default */
  flex-direction: row-reverse;
  flex-direction: column;
  flex-direction: column-reverse;
}
```

- **`justify-content`**: This property aligns the flex items along the main axis.

```css
.container {
  justify-content: flex-start; /* default */
  justify-content: flex-end;
  justify-content: center;
  justify-content: space-between;
  justify-content: space-around;
  justify-content: space-evenly;
}
```

- **`align-items`**: This property aligns the flex items along the cross axis.

```css
.container {
  align-items: stretch; /* default */
  align-items: flex-start;
  align-items: flex-end;
  align-items: center;
  align-items: baseline;
}
```

- **`flex-wrap`**: This property defines whether the flex items should wrap or not.

```css
.container {
  flex-wrap: nowrap; /* default */
  flex-wrap: wrap;
  flex-wrap: wrap-reverse;
}
```

### Flexbox Examples

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>

<style>
  .container {
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
  .item {
    background-color: lightblue;
    padding: 20px;
    margin: 10px;
  }
</style>
```

## Introduction to Grid

### What is CSS Grid?

CSS Grid Layout is a two-dimensional layout system for the web. It allows you to create complex layouts on the web easily, with rows and columns.

### Basic Grid Properties

- **`display: grid;`**: This property is applied to a container element to activate grid layout for its children.

```css
.container {
  display: grid;
}
```

- **`grid-template-columns`**: This property defines the columns of the grid.

```css
.container {
  grid-template-columns: 100px 100px 100px;
  grid-template-columns: 1fr 2fr;
  grid-template-columns: repeat(3, 1fr);
}
```

- **`grid-template-rows`**: This property defines the rows of the grid.

```css
.container {
  grid-template-rows: 50px 50px;
  grid-template-rows: 1fr 2fr;
  grid-template-rows: repeat(2, 1fr);
}
```

- **`gap`**: This property defines the gap between the rows and columns.

```css
.container {
  gap: 10px;
}
```

- **`grid-column` and `grid-row`**: These properties define the positioning of grid items.

```css
.item {
  grid-column: 1 / 3; /* spans from column 1 to column 3 */
  grid-row: 2 / 4; /* spans from row 2 to row 4 */
}
```

### Grid Examples

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <div class="item">Item 4</div>
</div>

<style>
  .container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 100px 100px;
    gap: 10px;
  }
  .item {
    background-color: lightgreen;
    padding: 20px;
    text-align: center;
  }
</style>
```

## Resources

Here are some additional resources to help you learn more about Flexbox and Grid:

- [MDN Web Docs - Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)
- [MDN Web Docs - CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
- [CSS Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Tricks - A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---

This README provides an overview of Lesson 3: Flexbox and Grid, covering the basics and examples of both layout techniques. For further learning, check out the provided resources and examples.