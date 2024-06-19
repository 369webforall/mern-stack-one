# CSS

## CSS CLASS RECORDING

1. [CSS Basic](https://youtu.be/7vBdrIH5BW0)

2. [CSS Basic- Box Model](https://youtu.be/ym8VB_uRP1w)

3. [CSS Basic- Flex Box](https://youtu.be/ZuzZxYdcfZw)

4. [CSS Basic- Layout exercise](https://youtu.be/R3QeSst58lo)

5. [CSS Basic- Layout exercise](https://youtu.be/AOyHjBnDc2c)

6. [CSS Basic- Layout exercise](https://youtu.be/v4uXK1NsUVg)

7. [CSS Basic- Layout exercise](https://youtu.be/0Q8UeQPKm90)

8. [CSS Basic- Layout exercise- CH-8](https://youtu.be/ONWSNTew3Zw)

9. [CSS Basic- Layout exercise- CH-8](https://youtu.be/F4RYnAEL4s8)

10. [CSS Basic- Layout exercise- CH-8-final](https://youtu.be/eqL-O0NiUfM)

11. [CSS Basic- CARD, Position properties](https://youtu.be/9JkwZKsK4q4)

12. [HTML form element](https://youtu.be/Ex5AymdR2Bs)


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

CSS Flexbox, or the Flexible Box Layout Module, is a CSS3 layout mode designed to help you arrange items within a container, even when their size is unknown or dynamic. Flexbox aims to provide a more efficient way to lay out, align, and distribute space among items in a container.

**Basic Concepts**

1. `Flex Container:` The parent element where the flex layout is applied. 
 It’s defined by setting display: flex or display: inline-flex.

```css
.container {
    display: flex;
}


```


2. `Flex Items:` The child elements inside the flex container. 
These are automatically adjusted to align and distribute space within the container.


**Flex Container Properties**

- `flex-direction:` Defines the direction in which the flex items are placed in the flex container.

    - `row (default):` left to right in ltr; right to left in rtl
    - `row-reverse:` right to left in ltr; left to right in rtl
    - `column:` top to bottom
    - `column-reverse:` bottom to top


```css
.container {
    flex-direction: row;
}
```

- `justify-content:` Aligns the flex items along the main axis (horizontal by default).

    - `flex-start (default):` items are packed toward the start of the flex-direction
    - `flex-end:` items are packed toward the end of the flex-direction
    - `center:` items are centered along the line
    - `space-between:` items are evenly distributed; first item is at the start, last item at the end
    - `space-around:` items are evenly distributed with space around them
    - `space-evenly:` items are distributed so that the spacing between any two items (and the space to the edges) is equal

```css
.container {
    justify-content: center;
}
```

- `align-items:` Aligns the flex items along the cross axis (vertical by default).

    - `stretch (default):` stretch to fill the container
    - `flex-start:` cross-start margin edge of the items is placed on the cross-start line
    - `flex-end:` cross-end margin edge of the items is placed on the cross-end line
    - `center:` items are centered in the cross-axis
    - `baseline:` items are aligned such as their baselines align

```css

.container {
    align-items: center;
}
```

`flex-wrap:` Defines whether the flex items should wrap or not, if there isn’t enough space in the flex container.

`nowrap (default):` all flex items will be on one line

`wrap:` flex items will wrap onto multiple lines, from top to bottom

`wrap-reverse:` flex items will wrap onto multiple lines from bottom to top


```css
.container {
    flex-wrap: wrap;
}
```


`align-content:` Aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.

`flex-start:` lines packed to the start of the container

`flex-end:` lines packed to the end of the container

`center:` lines packed to the center of the container

`space-between:` lines evenly distributed; the first line is at the start of the container while the last one is at the end

`space-around:` lines evenly distributed with equal space around each line

`stretch (default):` lines stretch to take up the remaining space

```css
.container {
    align-content: space-around;
}
```

**Flex Item Properties (children)**

`order:` Controls the order in which flex items appear in the flex container.

```css
.item {
    order: 2;
}
```

`flex-grow:` Defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates how much of the available space inside the flex container the item should take up.

```css
.item {
    flex-grow: 1;
}
```

`flex-shrink:` Defines the ability for a flex item to shrink if necessary. It also accepts a unitless value that serves as a proportion.

```css

.item {
    flex-shrink: 1;
}
```

`flex-basis:` Defines the default size of an element before the remaining space is distributed. It can be a length (e.g., 20%, 5rem, etc.) or auto.

```css

.item {
    flex-basis: 100px;
}
```

`align-self:` Allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

```css
.item {
    align-self: flex-end;
}
```
Example

Here is a complete example to illustrate Flexbox in action:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Example</title>
    <style>
        .container {
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: center;
            height: 100vh;
        }
        .item {
            background-color: lightcoral;
            padding: 20px;
            margin: 10px;
            flex-grow: 1;
            flex-shrink: 1;
            flex-basis: 100px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
    </div>
</body>
</html>
```

## CSS Position properties

CSS position properties are used to control the layout and positioning of HTML elements on a webpage. Understanding these properties is crucial for creating complex and responsive web designs. Here are the key position properties in CSS:

1. Static (default)

`position: static;`

- This is the default positioning for all HTML elements. Elements are positioned according to the normal flow of the document, meaning they appear in the order they are written in the HTML. They are not affected by top, right, bottom, or left properties.

```css
div {
  position: static; /* Default behavior */
}
```

2. Relative

`position: relative;`

- Elements are positioned relative to their normal position in the document flow. This means you can use top, right, bottom, and left properties to move the element from its original position without affecting the layout of surrounding elements. The space for the element in the normal flow is still preserved.

```css
div {
  position: relative;
  top: 20px;
  left: 30px;
}

```

3. Absolute

`position: absolute;`

- Elements are positioned relative to the nearest positioned ancestor (an ancestor with a position other than static). If there is no such ancestor, they are positioned relative to the initial containing block (usually the viewport). The top, right, bottom, and left properties are used to specify the exact position. Absolute positioning removes the element from the normal document flow, so it does not affect the position of other elements.

```css
div {
  position: absolute;
  top: 50px;
  left: 100px;
}

```

4. Fixed

`position: fixed;`

- Elements are positioned relative to the viewport and do not move when the page is scrolled. Like absolute positioning, fixed positioning removes the element from the normal document flow. The top, right, bottom, and left properties are used to specify the position relative to the viewport.

```css
div {
  position: fixed;
  top: 0;
  right: 0;
}

```

5. Sticky

`position: sticky;`

- Elements are positioned based on the user's scroll position. A sticky element toggles between relative and fixed positioning, depending on the scroll position. It is treated as relative until it crosses a specified threshold (using top, right, bottom, or left), after which it is treated as fixed. This is useful for creating headers or sidebars that stick to the top of the page when scrolled to.

```css
div {
  position: sticky;
  top: 10px; /* Sticks to the top of the container after scrolling 10px */
}

```

### Practical Use Cases
- Static: For elements that follow the normal flow of the document (e.g., paragraphs, headers).

- Relative: For slight adjustments of an element's position without affecting the surrounding elements (e.g., for small offsets or aligning elements within a container).

- Absolute: For elements that need to be placed exactly within a specific container or for overlays (e.g., dropdown menus, tooltips).

- Fixed: For elements that should stay in a fixed position relative to the viewport (e.g., navigation bars, back-to-top buttons).

- Sticky: For elements that should remain visible within the viewport while scrolling but only after reaching a certain scroll position (e.g., sticky headers or sidebars).


## form

**The <form> Element**

The <form> element defines an HTML form used for collecting user input. It is a container for different types of input elements, such as text fields, checkboxes, radio buttons, submit buttons, and more.

```html
<form action="URL" method="POST/GET">
  <!-- Form elements go here -->
</form>

```
`Attributes`
  - action: Specifies the URL where the form data will be sent for processing.
  - method: Specifies the HTTP method to be used when sending form data. Common values are:
  - GET: Appends the form data to the URL, suitable for non-sensitive data and retrieving data.
  - POST: Sends the form data as a part of the request body, suitable for sensitive data and data manipulation.

**Common Form Elements**
1. Text Input (<input type="text">)
Used for single-line text input.

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name">
```
2. Password Input (<input type="password">)
Used for entering passwords, hides the input text.

```html
<label for="pwd">Password:</label>
<input type="password" id="pwd" name="pwd">
```

3. Submit Button (<input type="submit" value="Submit">)
Used to submit the form.

```html
<input type="submit" value="Submit">
```

4. Radio Buttons (<input type="radio">)
Used for selecting one option from a group.

```html
<label for="male">Male:</label>
<input type="radio" id="male" name="gender" value="male">
<label for="female">Female:</label>
<input type="radio" id="female" name="gender" value="female">
```

5. Checkboxes (<input type="checkbox">)
Used for selecting multiple options independently.

```html
<label for="subscribe">Subscribe:</label>
<input type="checkbox" id="subscribe" name="subscribe" value="newsletter">
```

## Projects

[Google DOC - Practical exercise to complete](https://docs.google.com/document/d/144gpYdeVUQljEFQBK_-x5M4KSM3R9Dc7mLkQpQNFjwA/edit)