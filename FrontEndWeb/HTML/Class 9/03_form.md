# Form
An HTML Form is used to collect user input on a webpage.  
For example: login forms, registration forms, search boxes, feedback forms.  

The data entered by the user can be sent to a server for processing.

## `<form>` Tag
The `<form>` tag is used to create a form.

### Syntax
```html
<form action="server-file" method="method-type">
   form elements
</form>
```

### Example
```html
<form action="submit.php" method="post">
   Name: <input type="text">
</form>
```

### Attributes
Attribute	|Description
----------|-------------
action	|Where the form data is sent
method	|Method to send data (GET or POST)

--------------------------------------------------------------------------------------------------------------------------------------

## Input Tag
The <input> tag is used to create different input fields.

### Syntax
```html
<input type="type-name">
```

--------------------------------------------------------------------------------------------------------------------------------------

## Common Input Types
### Text Input  
Used to enter text.
```html
Name: <input type="text">
```

### Password Input
Used to enter password (hidden characters).
```html
Password: <input type="password">
```

### Radio Button
Used to select one option from multiple choices.
```html
Gender:
<input type="radio" name="gender"> Male
<input type="radio" name="gender"> Female
```

### Checkbox
Used to select multiple options.
```html
Hobbies:
<input type="checkbox"> Reading
<input type="checkbox"> Sports
```

### Submit Button
Used to submit the form.
```html
<input type="submit" value="Submit">
```

--------------------------------------------------------------------------------------------------------------------------------------

## Label Tag
The <label> tag is used to describe input fields.

### Example
```html
<label>Name:</label>
<input type="text">
```

--------------------------------------------------------------------------------------------------------------------------------------

## Textarea
Used for large text input like comments or feedback.

### Syntax
```html
<textarea rows="4" cols="30"></textarea>
```

### Example
```html
<textarea rows="5" cols="40">
Write your message
</textarea>
```

--------------------------------------------------------------------------------------------------------------------------------------

## Select (Dropdown)
Used to create a dropdown menu.

### Syntax
```html
<select>
   <option>Option</option>
</select>
```

### Example
```html
<select>
<option>India</option>
<option>USA</option>
<option>UK</option>
</select>
```

--------------------------------------------------------------------------------------------------------------------------------------

## Complete Example of HTML Form
```html
<!DOCTYPE html>
<html>
<body>

<h2>Registration Form</h2>

<form>

Name: <input type="text"><br><br>

Password: <input type="password"><br><br>

Gender:
<input type="radio" name="gender"> Male
<input type="radio" name="gender"> Female <br><br>

Hobbies:
<input type="checkbox"> Reading
<input type="checkbox"> Sports <br><br>

Country:
<select>
<option>India</option>
<option>USA</option>
<option>UK</option>
</select>

<br><br>

Message:
<textarea rows="4" cols="30"></textarea>

<br><br>

<input type="submit" value="Submit">

</form>

</body>
</html>
```
