# CSS

## CSS CLASS RECORDING

1. [CSS Basic](https://youtu.be/7vBdrIH5BW0)


CSS (Cascading Style Sheets) is a stylesheet language used for describing the presentation of a document written in HTML. It controls the layout of multiple web pages all at once. Here's a basic guide to CSS:

### Basic Syntax

CSS syntax consists of a selector and a declaration block.

```css
selector {
    property: value;
    property: value;
    ...
}
```
### Selectors 

Selectors are used to target HTML elements.

**Type Selector**

1. Name or tag 

```css
p {
    color: blue;
}
// This will select all <p> elements and set their text color to blue
```

2. Class Selector

```css
.className {
    font-size: 20px;
}

// This will select all elements with the class className.
```

3. ID Selector

```css

#idName {
    margin: 10px;
}

// This will select the element with the ID idName.
```

4. Universal Selector

```css
* {
    box-sizing: border-box;
}

// This will apply the box-sizing property to all elements.
```

5. Attribute Selector

```css
[type="text"] {
    border: 1px solid #000;
}

//This will select all input elements with the attribute type="text".

```

## Common Properties

Here are some commonly used CSS properties:

1. Color and Background

```css
color: red;
background-color: yellow;
background-image: url('image.jpg');


```

2. Text

```css
font-size: 16px;
font-family: Arial, sans-serif;
text-align: center;
font-weight: bold;
```

3. Box Model

```css
width: 100px;
height: 100px;
padding: 10px;
margin: 20px;
border: 1px solid #000;
```

4. Positioning

```css
position: relative;
top: 10px;
left: 20px;
```

5. Display

```css
display: block;
display: inline-block;
display: none;
```


Example
Here’s an example combining some of the basics:

### HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1 class="heading">Hello, World!</h1>
    <p>This is a paragraph.</p>
    <p id="special">This is a special paragraph.</p>
</body>
</html>
```


### CSS (styles.css):

```css
/* Type Selector */
p {
    color: green;
}

/* Class Selector */
.heading {
    font-size: 24px;
    color: blue;
}

/* ID Selector */
#special {
    font-style: italic;
    background-color: lightgray;
}

/* Universal Selector */
* {
    box-sizing: border-box;
}

/* Attribute Selector */
[type="text"] {
    border: 2px solid red;
}
```