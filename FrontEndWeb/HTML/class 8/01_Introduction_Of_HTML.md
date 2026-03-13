## What is HTML?
HTML (HyperText Markup Language) is the standard language used to create and structure web pages on the internet.  
It tells the web browser how to display text, images, links, tables, and other elements on a webpage.  

Example: When you open a website, the structure of that page is written in HTML.

## Why HTML is Important
HTML is important because it is the foundation of every website.

### Main reasons:
- Creates the structure of web pages
- Displays text, images, videos, links
- Works with CSS (for design) and JavaScript (for functionality)
- Supported by all web browsers

### Example stack:
- HTML → Structure
- CSS → Design / Styling
- JavaScript → Behavior / Logic

------------------------------------------------------------------------------------------------------------------------------------------------

### Basic Structure of an HTML Document
Every HTML page follows a basic structure.
```HTML
  <!DOCTYPE html>
  <html>
  <head>
      <title>My First Web Page</title>
  </head>
  
  <body>
      <h1>Hello World</h1>
      <p>This is my first HTML page.</p>
  </body>
  </html>
```
#### Explanation:
Tag	| Purpose
----|-------------
 `<!DOCTYPE html>`|Tells browser this is HTML5
`<html>`|Root element of HTML page
`<head>`|Contains title and meta information
`<title>`|Title shown in browser tab
`<body>`|Visible content of the webpage


### What are HTML Tags?
HTML uses tags to define elements.

#### Example:
    <p>This is a paragraph</p>

- <p> → opening tag
- </p> → closing tag
Some tags do not need closing tags.

Example:
```HTML
  <br>
  <hr>
  <img>
```

### Common HTML Tags (Very Important)
Tag	| Use
----|------
`<h1> to <h6>`	|Headings
`<p>`	|Paragraph
`<a>`	|Link
`<img>`	|Image
`<br>`	|Line break
`<hr>`	|Horizontal line
`<ul>`	|Unordered list
`<ol>`	|Ordered list
`<li>`	|List item
`<table>`	|Create table

Example:
```HTML
<h1>Welcome</h1>
<p>This is a website.</p>

<a href="https://google.com">Go to Google</a>
```

------------------------------------------------------------------------------------------------------------------------------------------------

### HTML Attributes
Attributes give extra information to tags.

#### Example:
```HTML
<a href="https://google.com">Visit Google</a>
```
##### Here:
- href → attribute
- It tells where the link goes.

#### Another example:
```HTML
<img src="image.jpg" alt="My Image">
```
#### Attributes:
- `src` → image location
- `alt` → description of image

## Features of HTML
✔ Easy to learn
✔ Platform independent
✔ Works with all browsers
✔ Used for building websites
✔ Supports multimedia

------------------------------------------------------------------------------------------------------------------------------------------------

# Comments
Comments are used to add notes or explanations in the HTML code.  
They are not displayed in the browser, but they help developers understand the code.

### Syntax
  <!-- This is a comment -->

### Example
```html
<!DOCTYPE html>
<html>
<body>

<!-- This is a heading -->
<h1>Welcome to My Website</h1>

<!-- This is a paragraph -->
<p>This is my first webpage.</p>

</body>
</html>
```

#### In this code:
- The text inside <!-- --> is a comment
- It will not appear on the webpage

## Uses of Comments
✔ Explain the code
✔ Make code easier to understand
✔ Temporarily hide code

### Example: Commenting Code
```html
<!-- <p>This paragraph is hidden</p> -->
```
This paragraph will not appear because it is inside a comment.

