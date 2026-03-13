# Teble Tag
The `<table>` tag in HTML is used to create tables to organize data in rows and columns.

##Basic Table Tags
Tag	|Meaning
-----|-------
`<table>`	|Creates a table
`<tr>`	|Table row
`<th>`	|Table heading (bold)
`<td>`	|Table data (cell)
  
### Syntax
```html
<table>
   <tr>
      <th>Heading1</th>
      <th>Heading2</th>
   </tr>

   <tr>
      <td>Data1</td>
      <td>Data2</td>
   </tr>
</table>
```

### Example
```html
<!DOCTYPE html>
<html>
<body>

<h2>Student Table</h2>

<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>Course</th>
  </tr>

  <tr>
    <td>Rahul</td>
    <td>20</td>
    <td>B.Tech</td>
  </tr>

  <tr>
    <td>Aman</td>
    <td>21</td>
    <td>BCA</td>
  </tr>

</table>

</body>
</html>
```

#### Output Concept
Name	|Age	|Course
------|------|-----
Rahul	|20	|B.Tech
Aman	|21	|BCA

## Important Attributes
- border → Adds border to the table
- cellpadding → Space inside cells
- cellspacing → Space between cells

### Example:
    <table border="1" cellpadding="10" cellspacing="5">
