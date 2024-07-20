# HTML

#### Doctype -  <!DOCTYPE html> 

This document is html

```html
<!DOCTYPE html>
<html>
	<head>
    	<title>Title</title>
	</head>
	<body>
		This is body
	</body>
</html>
```



#### HTML Headings

```html
<h1>This is heading1</h1>
<h2>This is heading2</h2>
<h3>This is heading3</h3>
<h4>This is heading4</h4>
<h5>This is heading5</h5>
<h6>This is heading6</h6>
```



#### HTML Paragraph

```html
<p> This is paragraph</p>
```



#### HTML links

```html
<a href="https://www.w3schools.com">Go to w3schools</a><br>
<a href="link1.html">Go to link1 html</a><br>
<a href="#heading1">Go to heading1</a><br>
```



#### HTML Elements

* An HTML element is defined by a start tag, some content, and an end tag.
* **Nested elements** - HTML elements can be nested (this means that elements can contain other elements).



#### HTML Attributes

HTML attributes provide additional information about HTML elements.

- All HTML elements can have **attributes**
- Attributes provide **additional information** about elements
- Attributes are always specified in **the start tag**
- Attributes usually come in name/value pairs like: **name="value"**

Example: href, src, height, width, style, title etc.



#### HTML text formatting

- `<b>` - Bold text

- `<strong>` - Important text

- `<i>` - Italic text

- `<em>` - Emphasized text

- `<mark>` - Marked text

- `<small>` - Smaller text

- `<del>` - Deleted text

- `<ins>` - Inserted text

- `<sub>` - Subscript text

- `<sup>` - Superscript text

- <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>



#### HTML comments

HTML comments are not displayed in the browser, but they can help document your HTML source code.

```html
    <!-- below code will not work -->
    <!--
         <p>X<sub>2</sub> text.</p>
        <p>X<sup>2</sup> text.</p>
    -->
```



#### HTML Image

```html
<img src="pic_trulli.jpg" alt="Italian Trulli">
<img src="img_chania.jpg" alt="Flowers in Chania" height="200" width="150">
```



#### HTML Favicon

A favicon is a small image displayed next to the page title in the browser tab.

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page Title</title>
  <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```



#### HTML Table

HTML tables allow web developers to arrange data into rows and columns.

```html
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```

- **Table cell** - Each table cell is defined by a `<td>` and a `</td>` tag.

- **Table row** - Each table row starts with a `<tr>` and ends with a `</tr>` tag.

- **Table header** - Sometimes you want your cells to be table header cells. In those cases use the `<th>` tag instead of the `<td>` tag

- **Caption** -  Defines a table caption

  ```html
  <table>
    <caption>Monthly savings</caption>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
  </table>
  ```

  

- **colgroup** - **col**  - Specifies a group of one or more columns in a table for formatting

  ```html
  <table>
    <colgroup>
      <col span="2" style="background-color:red">
      <col style="background-color:yellow">
    </colgroup>
    <tr>
      <th>ISBN</th>
      <th>Title</th>
      <th>Price</th>
    </tr>
    <tr>
      <td>3476896</td>
      <td>My first HTML</td>
      <td>$53</td>
    </tr>
  </table>
  ```

  

- **thead tbody tfooter**

  ```html
  <table>
    <thead>
      <tr>
        <th>Month</th>
        <th>Savings</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>January</td>
        <td>$100</td>
      </tr>
      <tr>
        <td>February</td>
        <td>$80</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <td>Sum</td>
        <td>$180</td>
      </tr>
    </tfoot>
  </table>
  ```

  

- **Table border** - HTML tables can have borders of different styles and shapes.

  ```html
  <!DOCTYPE html>
  <html>
  <head>
  <style>
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
  }
  </style>
  </head>
  <body>
  
  <h2>Collapsed Borders</h2>
  <p>If you want the borders to collapse into one border, add the CSS border-collapse property.</p>
  
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th> 
      <th>Age</th>
    </tr>
    <tr>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
    </tr>
    <tr>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
    </tr>
    <tr>
      <td>John</td>
      <td>Doe</td>
      <td>80</td>
    </tr>
  </table>
  
  </body>
  </html>
  
  
  ```

  - `dotted`   

  - `dashed`   

  - `solid`   

  - `double`   

  - `groove`   

  - `ridge`   

  - `inset`   

  - `outset`   

  - `none`   

  - `hidden`

    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    th, td {
      border-style: dotted;
    }
    </style>
    </head>
    <body>
    
    <h2>Table With Dotted Borders</h2>
    
    <p>Use the CSS border-style property to set the style of the borders.</p>
    
    <table style="width:100%">
      <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
      </tr>
      <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
      </tr>
      <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
      </tr>
      <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
      </tr>
    </table>
    
    </body>
    </html>
    
    
    ```

    

- **Table rowspan colspan**

  ```html
  <!DOCTYPE html>
  <html>
  <head>
  <style>
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
  }
  </style>
  </head>
  <body>
  
  <h2>Cell that spans two rows</h2>
  <p>To make a cell span more than one row, use the rowspan attribute.</p>
  
  <table style="width:100%">
    <tr>
      <th>Name</th>
      <td>Jill</td>
    </tr>
    <tr>
      <th rowspan="2">Phone</th>
      <td>555-1234</td>
    </tr>
    <tr>
      <td>555-8745</td>
    </tr>
  </table>
  </body>
  </html>
  
  
  ```

  

#### HTML Lists

- **Unorder list** - An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag. 

  - | disc   | Sets the list item marker to a bullet (default) |
    | ------ | ----------------------------------------------- |
    | circle | Sets the list item marker to a circle           |
    | square | Sets the list item marker to a square           |
    | none   | The list items will not be marked               |

  ```html
  <ul style="list-style-type:disc;">
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
  </ul> 
  ```

  ```html
  <!DOCTYPE html>
  <html>
  <body>
  
  <h2>A Nested List</h2>
  <p>Lists can be nested (list inside list):</p>
  
  <ul>
    <li>Coffee</li>
    <li>Tea
      <ul>
        <li>Black tea</li>
        <li>Green tea</li>
      </ul>
    </li>
    <li>Milk</li>
  </ul>
  
  </body>
  </html>
  
  
  ```

  

- **Order list** - An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.

  ```html
  <ol type="1" start="50">
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
  </ol>
  ```

  | Type     | Description                                                  |
  | :------- | :----------------------------------------------------------- |
  | type="1" | The list items will be numbered with numbers (default)       |
  | type="A" | The list items will be numbered with uppercase letters       |
  | type="a" | The list items will be numbered with lowercase letters       |
  | type="I" | The list items will be numbered with uppercase roman numbers |
  | type="i" | The list items will be numbered with lowercase roman numbers |

  

- **Description list** - 

  A description list is a list of terms, with a description of each term.

  The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term

  ```html
  <dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
  </dl>
  ```

  

#### HTML DIV

The `<div>` element is used as a container for other HTML elements.

```html
<!DOCTYPE html>
<html>
<style>
div {
  background-color: #FFF4A3;
}
</style>
<body>

<h1>HTML DIV Example</h1>

<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>

<p>The yellow background is added to demonstrate the footprint of the DIV element.</p>

</body>
</html>
```



#### HTML Iframe

An HTML iframe is used to display a web page within a web page.

```html
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
```
