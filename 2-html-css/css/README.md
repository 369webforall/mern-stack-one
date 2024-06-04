# CSS

## CSS CLASS RECORDING

1. [CSS Basic](https://youtu.be/7vBdrIH5BW0)

2. [CSS Basic- Box Model](https://youtu.be/ym8VB_uRP1w)


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

## BOX MODEL

**Components of the CSS Box Model**

1. Content Box:

- This is the area where the content of the element, such as text, images, or other media, is displayed.
- The size of the content box can be adjusted using the width and height properties in CSS.

2. Padding:

- Padding is the space between the content and the border of the element.
- It creates an inner space inside the element, but outside the content.
- Padding can be set using the padding property, which can take individual values for each side (top, right, bottom, left) or a single value to apply equally to all sides.

3. Border:

- The border wraps around the padding and the content.
- It can be styled using properties such as border-width, border-style, and border-color.
- Borders can also have individual settings for each side or a shorthand to set all at once.

4. Margin:

- Margin is the space outside the border, separating the element from other elements.
- Margins can be set using the margin property, which can also accept individual values for each side or a shorthand value.
- Margins can collapse, meaning the vertical margins of adjacent elements might combine to form a single margin.

example

```css
.box {
  width: 200px;
  height: 100px;
  padding: 20px;
  border: 10px solid black;
  margin: 30px;
}

```

`For an element with the class box, the total size calculation is:`

Content: 200px (width) x 100px (height)

- Padding: 20px on all sides
- Border: 10px on all sides
- Margin: 30px on all sides
- The total width and height including padding and border would be:

- Width: 200px (content) + 20px (left padding) + 20px (right padding) + 10px (left border) + 10px (right border) = 260px
- Height: 100px (content) + 20px (top padding) + 20px (bottom padding) + 10px (top border) + 10px (bottom border) = 160px

`Box-Sizing Property`

The box-sizing property can change how the size of an element is calculated. It has two main values:

`content-box (default):`

The width and height properties include only the content, not padding, border, or margin.

`border-box:`

The width and height properties include content, padding, and border, but not margin.

```css
.box {
  box-sizing: border-box;
}

```

## FLEX BOX

