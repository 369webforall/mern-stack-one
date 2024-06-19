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


6. Dropdown List (<select>)
Used for selecting an option from a dropdown list.

```html
<label for="car">Select Car:
<select id="cars" name="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </select>
    
</label>
```

7. Text Area (<textarea>)
Used for multi-line text input.

```html

<label for="message">Message:</label>
<textarea id="message" name="message"></textarea>

```

**Example Form**
Here’s an example of a complete form:

```html

<form action="/submit-form" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name"><br><br>
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
  
  <label for="pwd">Password:</label>
  <input type="password" id="pwd" name="pwd"><br><br>
  
  <label for="gender">Gender:</label>
  <input type="radio" id="male" name="gender" value="male"> Male
  <input type="radio" id="female" name="gender" value="female"> Female<br><br>
  
  <label for="subscribe">Subscribe:</label>
  <input type="checkbox" id="subscribe" name="subscribe" value="newsletter"><br><br>
  
  <label for="cars">Choose a car:</label>
  <select id="cars" name="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </select><br><br>
  
  <label for="message">Message:</label>
  <textarea id="message" name="message"></textarea><br><br>
  
  <input type="submit" value="Submit">
</form>
```

### form project code for practice

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
        <legend>Account type (required)</legend>
        <label for="personal-account"><input id="personal-account" type="radio" name="account-type" class="inline" checked /> Personal</label>
        <label for="business-account"><input id="business-account" type="radio" name="account-type" class="inline" /> Business</label>
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
      <label for="terms-and-conditions">
        <input class="inline" id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" /> I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a>
      </label>
      <input type="submit" value="Submit" />
    </form>
  </body>
</html>
```

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

.inline{
  display: inline; 
}

```