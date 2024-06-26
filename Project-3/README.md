# CSS Color Markers

This project showcases a simple webpage displaying colored marker illustrations using HTML and CSS. The project includes a header, a container with three markers, and a footer reference. Each part of the HTML and CSS code is explained below.

## HTML Code

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colored Markers</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <h1>CSS Color Markers</h1>
    <div class="container">
      <div class="marker red">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker green">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker blue">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
    </div>
    <p class="reference">Made with <span class="heart">❤</span> by <a href="https://www.linkedin.com/in/itzmudassir/">Mudassir</a></p>
  </body>
</html>
```

### HTML Explanation

- **`<!DOCTYPE html>`**: This declaration defines the document type and version of HTML. It helps the browser to render the webpage correctly.
- **`<html lang="en">`**: The root element of the HTML document with the language set to English.
- **`<head>`**: Contains meta-information about the HTML document, such as character set, viewport settings, title, and link to the CSS stylesheet.
  - **`<meta charset="utf-8">`**: Specifies the character encoding for the document.
  - **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Sets the viewport to ensure the page is responsive on all devices.
  - **`<title>`**: Defines the title of the document displayed in the browser tab.
  - **`<link rel="stylesheet" href="styles.css">`**: Links to the external CSS file for styling.
- **`<body>`**: Contains the content of the HTML document.
  - **`<h1>CSS Color Markers</h1>`**: A header element with the title of the page.
  - **`<div class="container">`**: A container div holding the marker elements.
    - **`<div class="marker red">`**: A div for the red marker with nested divs for the cap and sleeve.
    - **`<div class="marker green">`**: A div for the green marker with nested divs for the cap and sleeve.
    - **`<div class="marker blue">`**: A div for the blue marker with nested divs for the cap and sleeve.
  - **`<p class="reference">Made with <span class="heart">❤</span> by <a href="https://www.linkedin.com/in/itzmudassir/">Mudassir</a></p>`**: A footer paragraph with a reference to the creator and a link to their LinkedIn profile.

## CSS Code

```css
h1 {
  text-align: center;
  font-family: 'Roboto', sans-serif;
}

.container {
  background-color: rgb(255, 255, 255);
  padding: 10px 0;
}

.marker {
  width: 200px;
  height: 25px;
  margin: 10px auto;
}

.cap {
  width: 60px;
  height: 25px;
}

.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, 0.5);
  border-left: 10px double rgba(0, 0, 0, 0.75);
}

.cap, .sleeve {
  display: inline-block;
}

.red {
  background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
  box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
  border-radius: 5px;
}

.green {
  background: linear-gradient(#55680D, #71F53E, #116C31);
  box-shadow: 0 0 20px 0 #3B7E20CC;
  border-radius: 5px;
}

.blue {
  background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
  box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);
  border-radius: 5px;
}

.reference {
  text-align: center;
  font-size: 0.8em;
  color: #555;
  font-family: 'Roboto', sans-serif;
}

.reference a {
  color: #dd0e0e;
  text-decoration: none;
}

.reference a:hover {
  color: #f00;
}

.reference span {
  color: #f00;
}
```

### CSS Explanation

- **`h1`**: Styles the header element.
  - **`text-align: center;`**: Centers the text horizontally.
  - **`font-family: 'Roboto', sans-serif;`**: Sets the font family to Roboto.
- **`container`**: Styles the container div.
  - **`background-color: rgb(255, 255, 255);`**: Sets the background color to white.
  - **`padding: 10px 0;`**: Adds padding at the top and bottom.
- **`marker`**: Styles the marker div.
  - **`width: 200px;`**: Sets the width of the marker.
  - **`height: 25px;`**: Sets the height of the marker.
  - **`margin: 10px auto;`**: Centers the marker and adds margin above and below.
- **`cap`**: Styles the cap div.
  - **`width: 60px;`**: Sets the width of the cap.
  - **`height: 25px;`**: Sets the height of the cap.
- **`sleeve`**: Styles the sleeve div.
  - **`width: 110px;`**: Sets the width of the sleeve.
  - **`height: 25px;`**: Sets the height of the sleeve.
  - **`background-color: rgba(255, 255, 255, 0.5);`**: Sets the background color with opacity.
  - **`border-left: 10px double rgba(0, 0, 0, 0.75);`**: Adds a double border to the left side.
- **`.cap, .sleeve`**: Common styles for cap and sleeve.
  - **`display: inline-block;`**: Displays the elements inline but allows them to have block properties.
- **`.red`**: Styles the red marker.
  - **`background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));`**: Sets a linear gradient background.
  - **`box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);`**: Adds a shadow effect.
  - **`border-radius: 5px;`**: Rounds the corners.
- **`.green`**: Styles the green marker.
  - **`background: linear-gradient(#55680D, #71F53E, #116C31);`**: Sets a linear gradient background.
  - **`box-shadow: 0 0 20px 0 #3B7E20CC;`**: Adds a shadow effect.
  - **`border-radius: 5px;`**: Rounds the corners.
- **`.blue`**: Styles the blue marker.
  - **`background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));`**: Sets a linear gradient background.
  - **`box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);`**: Adds a shadow effect.
  - **`border-radius: 5px;`**: Rounds the corners.
- **`.reference`**: Styles the reference paragraph.
  - **`text-align: center;`**: Centers the text horizontally.
  - **`font-size: 0.8em;`**: Sets the font size.
  - **`color: #555;`**: Sets the text color.
  - **`font-family: 'Roboto', sans-serif;`**: Sets the font family to Roboto.
- **`.reference a`**: Styles the anchor tag within the reference paragraph.
  - **`color:

 #dd0e0e;`**: Sets the link color.
  - **`text-decoration: none;`**: Removes the underline from the link.
- **`.reference a:hover`**: Styles the anchor tag on hover.
  - **`color: #f00;`**: Changes the link color on hover.
- **`.reference span`**: Styles the span within the reference paragraph.
  - **`color: #f00;`**: Sets the text color.

This README explains each part of the HTML and CSS code used to create the colored markers project. By understanding the structure and styling, you can create similar projects and expand your CSS skills.