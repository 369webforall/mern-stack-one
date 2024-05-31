# HTML-CSS

## CLASS RECORDING VIDEO LINK

1. [HTML CLASS](https://youtu.be/tQ8YtXxsGOA)


# HTML - Hypertext Markup Language

- Describes the structure of a Web page

## LEVEL ONE

  **Two things you must understand in high level**

1. Tags / html file
2. Attributes
3. commnets in html

**What is HTML?**

- HTML stands for Hyper Text Markup Language
- HTML is the standard markup language for creating Web pages
- HTML describes the structure of a Web page
- HTML consists of a series of elements
- HTML elements tell the browser how to display the content
- HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

## Basic HTML page

```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<ul>
<li>One</li>
<li>Two</li>
<li>Three</li>
</ul>

<ol>
<li>One</li>
<li>Two</li>
<li>Three</li>
</ol>

<img src="image link" alt="image text" />

<a href="link">Home</a>

<hr />

<br />


</body>
</html>

```

![HTML Element](./images/1.png)

## Empty Element

Insert or Embed something in the document
`<input>, <img>, <br>, <hr>, <embed>, <meta>, <link>`

## Nesting

HTML elements can be nested

```
    <div class="list">
    <h2>My List: </h2>
    <ul>
        <li>Apple</li>
        <li>Mango</li>
        <li>Banana</li>
    </ul>
    </div>

```

## Attributes

Attributes contain extra information about the element that won't appear in the content

`<img src="https://images.unsplash.com/photo-1502082553048-f009c37129b9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80" width="100"/>`

- All HTML elements can have attributes
- Attributes provide additional information about elements
- Attributes are always specified in the start tag
- Attributes usually come in name/value pairs like: name="value"

## Boolean Attributes

- some attributes can be written without value eg. disabled is boolean attributes
  `<button onclick="alert("button clicked") disabled="disabled">Button Click</button>`
  `<button onclick="alert("button clicked") disabled >Button Click</button>`

## Most common HTML Elements

There are hundreds of HTML elements, most of the time we only use these elemets.

### Define a section: `<header>, <footer>, <nav>, <main>, <section>, <div>`

### Define a text content: `<h1> to <h6>, <p>, <span>, <ul>, <li>, <ol>`

### Define a form or a input: `<form>, <input>, <button>, <lable>, <textarea>`

### Define a img or a link: `<img>, <a>`

### Others: `<hr >, <br>`

## Block-level vs inline elements

![Block-level vs inline elements](./images/2-block.png)

## Most common inline elements are colored.

![Most common inline elements](./images/3-block.png)

## Description about tags in head section

![Head Section](./images/4.head.png)

## Practice how inline and block element behave.

## Best Practice -sample code from freecode camp


```html
<body>
    <main>
      <h1>CatPhotoApp</h1>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
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
      <p>
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>
  </body>
</html>

```

## Table

`<table>:`

The container element for the table.

`<tr> (Table Row):`
Defines a row in the table. It contains <th> or <td> elements.


<tr>
  <td>Row 1, Cell 1</td>
  <td>Row 1, Cell 2</td>
</tr>

`<th> (Table Header Cell):`
Defines a header cell in a table, usually used at the start of a row or column. Text in <th> elements is typically bold and centered by default.


<tr>
  <th>Header 1</th>
  <th>Header 2</th>
</tr>

`<td> (Table Data Cell):`
Defines a standard data cell in a table.

<tr>
  <td>Data 1</td>
  <td>Data 2</td>
</tr>
Optional HTML Table Tags

`<thead> (Table Head):`
Groups a set of rows that define the head of the table. It usually contains header information.

<thead>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
</thead>

`<tbody> (Table Body):`
Groups a set of rows that contain the main body of the table data.


<tbody>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</tbody>

`<tfoot> (Table Footer):`

Groups a set of rows that define the footer of the table.


<tfoot>
  <tr>
    <td>Footer 1</td>
    <td>Footer 2</td>
  </tr>
</tfoot>
<caption>:
Provides a caption or title for the table.


<caption>Table Title</caption>

`<colgroup> and <col>:`
The <colgroup> element groups one or more <col> elements, which define column properties for the table.


<colgroup>
  <col style="background-color: yellow">
  <col style="background-color: lightblue">
</colgroup>

`Attributes for Table Elements`

- border: Specifies the width of the border around the table.
- cellpadding: Defines the space between the cell wall and the cell content.
- cellspacing: Defines the space between cells.
- width: Specifies the width of the table.
- align: Aligns the table to the left, right, or center.

Example of a Complete HTML Table

```html
<table border="1">
  <caption>Monthly Sales Data</caption>
  <thead>
    <tr>
      <th>Month</th>
      <th>Sales</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$10,000</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$8,000</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td>
      <td>$18,000</td>
    </tr>
  </tfoot>
</table>
```
Explanation of Example

- <table border="1">: Creates a table with a border.
- <caption>: Adds a title to the table, "Monthly Sales Data".
- <thead>: Contains the header row with columns "Month" and "Sales".
- <tbody>: Contains the data rows for January and February.
- <tfoot>: Contains the footer row with the total sales.


## Form

`The <form> Element`

The <form> element is the container for all form controls. It has several important attributes:

- action: Specifies the URL to which the form data will be sent.
- method: Defines the HTTP method to be used when sending the form data. Common values are GET and POST.
- enctype: Specifies how the form data should be encoded when submitted. Common values are application/x-www-form-urlencoded (default) and multipart/form-data (used for file uploads).
Important Form Tags

`<input>:`
The <input> element is used to create various types of form controls. Important attributes include:

- type: Specifies the type of input control. Common types are:
- text: Single-line text input
- password: Password input (text is hidden)
- email: Input for email addresses
- number: Numeric input
- checkbox: Checkbox input
- radio: Radio button input
- submit: Submit button
- reset: Reset button
- file: File upload control
- hidden: Hidden input
- name: Name of the form control, used to identify the data after form submission.
- value: The initial value of the input control.

`<label>:`
The <label> element defines a label for an <input> element. The for attribute associates the label with a specific input element by its id.

<label for="username">Username:</label>
<input type="text" id="username" name="username">

`<textarea>:`
The <textarea> element is used for multi-line text input.


<textarea name="message" rows="4" cols="50"></textarea>

`<select>:`
The <select> element creates a drop-down list. It contains <option> elements.


<select name="country">
  <option value="usa">USA</option>
  <option value="canada">Canada</option>
</select>

`<option>:`
The <option> element defines an option in a drop-down list.


<option value="usa">USA</option>

`<button>:`
The <button> element is used to create a clickable button.


<button type="submit">Submit</button>

`<fieldset> and <legend>:`

The <fieldset> element groups related form controls, and the <legend> element provides a caption for the fieldset.


<fieldset>
  <legend>Personal Information</legend>
  <label for="fname">First Name:</label>
  <input type="text" id="fname" name="fname">
</fieldset>

`<datalist>:`
The <datalist> element provides a list of predefined options for an <input> element.


<input list="browsers" name="browser">
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
</datalist>

`<output>:`
The <output> element represents the result of a calculation or user action.

<output name="result" for="a b">0</output>


## Example of a Complete Form

```html
<form action="/submit" method="post">
  <fieldset>
    <legend>Personal Information</legend>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="50"></textarea>
  </fieldset>
  
  <fieldset>
    <legend>Preferences</legend>
    <label for="newsletter">Subscribe to newsletter:</label>
    <input type="checkbox" id="newsletter" name="newsletter">
    
    <label for="gender">Gender:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label>
  </fieldset>
  
  <button type="submit">Submit</button>
  <button type="reset">Reset</button>
</form>
```

## Registration form

- index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Registration Form</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form method="post" action='https://register-demo.freecodecamp.org'>
      <fieldset>
        <label for="first-name">Enter Your First Name: <input id="first-name" name="first-name" type="text" required /></label>
        <label for="last-name">Enter Your Last Name: <input id="last-name" name="last-name" type="text" required /></label>
        <label for="email">Enter Your Email: <input id="email" name="email" type="email" required /></label>
        <label for="new-password">Create a New Password: <input id="new-password" name="new-password" type="password" pattern="[a-z0-5]{8,}" required /></label>
      </fieldset>
      <fieldset>
        <label for="personal-account"><input id="personal-account" type="radio" name="account-type" class="inline" /> Personal Account</label>
        <label for="business-account"><input id="business-account" type="radio" name="account-type" class="inline" /> Business Account</label>
        <label for="terms-and-conditions">
          <input id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" class="inline" /> I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a>
        </label>
      </fieldset>
      <fieldset>
        <label for="profile-picture">Upload a profile picture: <input id="profile-picture" type="file" name="file" /></label>
        <label for="age">Input your age (years): <input id="age" type="number" name="age" min="13" max="120" /></label>
        <label for="referrer">How did you hear about us?
          <select id="referrer" name="referrer">
            <option value="">(select one)</option>
            <option value="1">freeCodeCamp News</option>
            <option value="2">freeCodeCamp YouTube Channel</option>
            <option value="3">freeCodeCamp Forum</option>
            <option value="4">Other</option>
          </select>
        </label>
        <label for="bio">Provide a bio:
          <textarea id="bio" name="bio" rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>
        </label>
      </fieldset>
      <input type="submit" value="Submit" />
    </form>
  </body>
</html>


```

- style.css

```css
body {
  width: 100%;
  height: 100vh;
  margin: 0;
  background-color: #1b1b32;
  color: #f5f6f7;
  font-family: Tahoma;
  font-size: 16px;
}

h1, p {
  margin: 1em auto;
  text-align: center;
}

form {
  width: 60vw;
  max-width: 500px;
  min-width: 300px;
  margin: 0 auto;
  padding-bottom: 2em;
}

fieldset {
  border: none;
  padding: 2rem 0;
  border-bottom: 3px solid #3b3b4f;
}

fieldset:last-of-type {
  border-bottom: none;
}

label {
  display: block;
  margin: 0.5rem 0;
}

input,
textarea,
select {
  margin: 10px 0 0 0;
  width: 100%;
  min-height: 2em;
}

input, textarea {
  background-color: #0a0a23;
  border: 1px solid #0a0a23;
  color: #ffffff;
}

.inline {
  width: unset;
  margin: 0 0.5em 0 0;
  vertical-align: middle;
}

input[type="submit"] {
  display: block;
  width: 60%;
  margin: 1em auto;
  height: 2em;
  font-size: 1.1rem;
  background-color: #3b3b4f;
  border-color: white;
  min-width: 300px;
}

input[type="file"] {
  padding: 1px 2px;
}
a {
    color: #dfdfe2;
}
```


### Create basic html page structure for below Projects, Try to use semantic tags as possible. css not required.

Just create the structure of the page.

# Project -1

- No css only structure of the page

[cake recipe](https://www.allrecipes.com/recipe/241038/microwave-chocolate-mug-cake/)

# Project - 2

- No css only structure of the page

[tribute-page](https://tribute-page.freecodecamp.rocks/)

# Project - 3

[Personal-portfolio](https://personal-portfolio.freecodecamp.rocks/)

# Project - 4

[product-landing-page](https://product-landing-page.freecodecamp.rocks/)

# Project - 5

[mytunes](https://jolly-kalam-23776e.netlify.app/mytunes/)

# Project - 6

[resturant-page](https://jolly-kalam-23776e.netlify.app/restaurantwebsite/)

# Project - 7

[photographysite](https://jolly-kalam-23776e.netlify.app/photographysite/#images)

# More project

[frontendmentor](https://www.frontendmentor.io/challenges?sort=difficulty|asc&types=free)

# Resoureces

[HTML Dog Tag List](http://www.htmldog.com/reference/htmltags/)
[W3Schools Tag List](http://www.w3schools.com/tags/default.asp)
[Quackit HTML Tag List](http://www.quackit.com/html/tags/)
