# HTML Anchor Tag 🔗
The Anchor tag (<a>) is used to create links (hyperlinks) in a webpage. It allows users to move from one page to another page, website, or location.

### Syntax
    <a href="URL">Link Text</a>
- <a> → Anchor tag
- href → Hyperlink reference (the destination link)
- Link Text → Text users click on

### Example 1: Link to another website
    <a href="https://www.google.com">Go to Google</a>
When the user clicks Go to Google, it opens the Google website.

### Example 2: Link to another page
    <a href="about.html">About Us</a>
This opens the about.html page.

### Example 3: Open link in new tab
    <a href="https://www.youtube.com" target="_blank">Open YouTube</a>
target="_blank" → Opens the link in a new tab.

### Example 4: Email link
    <a href="mailto:example@gmail.com">Send Email</a>
Clicking this opens the email application.

## Important Attributes
Attribute	|Description
----------|-----------
href	|Specifies the link destination
target	|Specifies where to open the link
title	|Shows extra information when hovering

## Full Example
```html
<!DOCTYPE html>
<html>
<body>

<h1>My Website</h1>

<a href="https://www.google.com">Visit Google</a><br>
<a href="about.html">About Page</a><br>
<a href="https://youtube.com" target="_blank">Open YouTube</a>

</body>
</html>
```
