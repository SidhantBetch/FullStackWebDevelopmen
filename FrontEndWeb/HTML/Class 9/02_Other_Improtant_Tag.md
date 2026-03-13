# `<div>` Tag
`div` stands for division.  
It is used to group elements together so they can be styled or managed easily.

### Syntax
```html
<div>
   content
</div>
```
### Example
```html
<div>
   <h1>Welcome</h1>
   <p>This is my website.</p>
</div>
```
The div tag is mainly used for layout and grouping elements.

----------------------------------------------------------------------------------------------------------------------------------------------------------

# `<section>` Tag
section is a semantic HTML tag used to define a separate section of a webpage.  

Examples of sections:
- Introduction
- About
- Services
- Contact

### Syntax
```html
<section>
   content
</section>
```
### Example
```html
<section>
   <h2>About Us</h2>
   <p>We build websites.</p>
</section>
```

----------------------------------------------------------------------------------------------------------------------------------------------------------

## Difference from div:
- div → generic container
- section → meaningful content section

----------------------------------------------------------------------------------------------------------------------------------------------------------

# class Attribute
class is used to apply the same style to multiple elements.

### Syntax
```html
<tag class="classname">
```

### Example
```html
<p class="text">Hello</p>
<p class="text">Welcome</p>
```
Both paragraphs have the same class, so they can share the same CSS style.

### Example with CSS:
```html
<style>
.text{
   color: blue;
}
</style>

<p class="text">Hello</p>
<p class="text">World</p>
```

----------------------------------------------------------------------------------------------------------------------------------------------------------

# id Attribute
id is used to identify one unique element in a webpage.

### Syntax
```html
<tag id="name">
```

### Example
```html
<h1 id="title">My Website</h1>
```

### Example with CSS:
```html
<style>
#title{
   color: red;
}
</style>

<h1 id="title">Welcome</h1>
```

----------------------------------------------------------------------------------------------------------------------------------------------------------

# Difference Between class and id
Feature	|class	|id
--------|-------|-------
Usage	|Multiple elements	|One element
Symbol in CSS	|.	|#
Example	|.box	|#header

Example:
```html
<div class="box">Box 1</div>
<div class="box">Box 2</div>

<div id="header">Header Section</div>
```

----------------------------------------------------------------------------------------------------------------------------------------------------------

# Complete Example
```html
<!DOCTYPE html>
<html>
<head>
<style>

.box{
   background-color: lightblue;
}

#main{
   color: red;
}

</style>
</head>

<body>

<section id="main">
<h1>Welcome</h1>
</section>

<div class="box">
<p>This is box 1</p>
</div>

<div class="box">
<p>This is box 2</p>
</div>

</body>
</html>
```
