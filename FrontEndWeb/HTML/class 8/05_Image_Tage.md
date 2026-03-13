# HTML Image Tag
The Image tag (<img>) is used to display images on a webpage.  
Unlike many HTML tags, the image tag is a self-closing tag, which means it does not need a closing tag.

### Syntax
    <img src="image_path" alt="description">

---------------------------------------------------------------------------------------------------------------------------------------

## Attributes:
- src (source) → Specifies the path of the image
- alt (alternative text) → Describes the image if it cannot be displayed

### Example 1: Display an Image
    <img src="photo.jpg" alt="Nature Image">
This will display the image photo.jpg on the webpage.

### Example 2: Image from Internet
    <img src="https://example.com/image.jpg" alt="Sample Image">
This loads the image from a website URL.

### Example 3: Set Width and Height
    <img src="photo.jpg" alt="Nature Image" width="300" height="200">
This sets the image size.

---------------------------------------------------------------------------------------------------------------------------------------

## Full Example
```html
<!DOCTYPE html>
<html>
<body>

<h2>My Image</h2>

<img src="nature.jpg" alt="Beautiful Nature" width="400" height="250">

</body>
</html>
```
