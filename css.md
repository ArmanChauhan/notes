# CSS



### Where to put CSS?

1. Inline CSS
2. Internal CSS
3. External CSS



##### Inline CSS

```html
<div style="width: 30%; height: 500px;">  <!-- This is inline CSS -->
</div>
```



##### Internal CSS

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Internal CSS</title>
        <style>
            .container {
                width: 30%;
                height: 500px;
                color: red;
            }
        </style>
    </head>
    <body>
        <div class="container">
		    This is example of internal CSS
		</div>
    </body>
</html>
```



##### External CSS

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Internal CSS</title>
        <link href="my_css.css" rel="stylesheet">
    </head>
    <body>
       <div class="container">
		    This is example of internal CSS
		</div> 
    </body>
</html>
```



### Color and Background color

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Internal CSS</title>
        <style>
            .container {
                color: red;
                background-color: green;
            }
        </style>
    </head>
    <body>
        <div class="container">
		    This is example of internal CSS
		</div>
    </body>
</html>
```



### CSS Selector

- Element selector
- CSS class selector
- CSS ID selector
- CSS Universal selector
- CSS Grouping selector

##### Element selector

```css
p {
	text-align: center;
	color: red;
}
```

##### CSS class selector

```css
.container {
	text-align: center;
	color: red;
}
```

##### CSS ID selector

```css
#container {
	text-align: center;
	color: red;
}
```

##### CSS Universal selector

```css
* {
	text-align: center;
	color: red;
}
```

##### CSS Grouping selector

```css
h1, h2, p {
	text-align: center;
	color: red;
}
```



### Border

```html
<DOCTYPE html>
<html>
	<head>
        <title>Border</title>
    </head>    
    <body>
        <div style="border: 10px solid red;">
            This is border example
        </div>
        <div style="border-left: 10px solid red;">
            This is border example
        </div>
         <div style="border-right: 10px solid red;">
            This is border example
        </div>
        <div style="border-top: 10px solid red;">
            This is border example
        </div>
        <div style="border-bottom: 10px double red;">
            This is border example
        </div>
    </body>
</html>
```

- dotted
- dashed
- solid
- double
- groove
- ridge
- groove
- inset
- outset
- none
- hidden



### Outline

CSS has the following outline properties:

- `outline-style`
- `outline-color`
- `outline-width`
- `outline-offset`
- `outline`

##### CSS Outline Style

The `outline-style` property specifies the style of the outline, and can have one of the following values:

- `dotted` - Defines a dotted outline
- `dashed` - Defines a dashed outline
- `solid` - Defines a solid outline
- `double` - Defines a double outline
- `groove` - Defines a 3D grooved outline
- `ridge` - Defines a 3D ridged outline
- `inset` - Defines a 3D inset outline
- `outset` - Defines a 3D outset outline
- `none` - Defines no outline
- `hidden` - Defines a hidden outline

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Outline</title>
    </head>
    <body>
        <div style="border: 10px solid red; outline: 12px solid green; outline-offset: 10px;">
            This is an example of border and outline
        </div>
    </body>
</html>
```



### Padding

CSS has the following padding properties:

- `padding`
- `padding-left`
- `padding-right`
- `padding-top`
- `padding-bottom`

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Padding</title>
    </head>
    <body>
        <div style="padding: 10px">
            This is padding 10 px
        </div>
        <div style="padding: 10px 15px 20px 25px;">
            This is padding 10 px
        </div>
        <div style="padding-left: 30px;">
            This is padding 10 px
        </div>
    </body>
</html>
```



### Margin

CSS has the following margin properties:

- `margin`
- `margin-left`
- `margin-right`
- `margin-top`
- `margin-bottom`

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Margin</title>
    </head>
    <body>
        <div style="border: 10px solid red; margin: 10px;">
            This is example of margin
        </div>
    </body>
</html>
```



### Height and Width

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Width-Height</title>
    </head>
    <body>
        <div style="border: 10px solid red; width: 50%; height: 500px;">
            This is example of height and width
        </div>
    </body>
</html>
```



### Min-width, max-width

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Width</title>
    </head>
    <body>
        <div style="border: 10px solid red; min-width: 50%; max-width: 70%;">
            This is example of min-width max width
        </div>
    </body>
</html>
```



### Min-height, max-height

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Height</title>
    </head>
    <body>
        <div style="border: 10px solid red; min-height: 200px; max-height: 500px;">
            This is example of min-height and max-height
        </div>
    </body>
</html>
```



### Box sizing

It keeps the same width including padding and margin

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Box sizing</title>
    </head>
    <body>
        <div style="border: 10px solid red; padding: 10px; margin: 10px; box-sizing: border-box">
            This is example of box sizing
        </div>
    </body>
</html>
```



### Overflow

- hidden   (default)
- scroll
- auto
- visible



- overflow
- overflow-x
- overflow-y



```html
<!DOCTYPE html>
<html>
    <head>
        <title>Overflow</title>
    </head>
    <body>
        <div style="border: 10px solid red; width: 500px; height: 500px; overflow: auto;">
            This is example of overflow
        </div>
    </body>
</html>
```



### Border radius

- border-radius
- border-top-left-radius
- border-top-right-radius
- border-bottom-left-radius
- border-bottom-right-radius



```html
<!DOCTYPE html>
<html>
    <head>
        <title>Borderradius</title>
    </head>
    <body>
        <div style="border: 10px solid red; border-radius: 10px;">
            This is example of border radius
        </div>
        <div style="border: 10px solid red; border-radius: 10px 15px 20px 25px;">
            This is example of border radius
        </div>
        <div style="border: 10px solid red; border-radius: 10px 0px 0px 0px;">
            This is example of border radius
        </div>
    </body>
</html>
```



### Box shadow

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Box shadow</title>
    </head>
    <body>
        <div style="border: 10px solid red; box-shadow: 10px 10px 3px red;">
            This is example of box shadow
        </div>
        <div style="border: 10px solid red; border-radius: -10px -15px 3px green;">
            This is example of box shadow
        </div>
        <div style="border: 10px solid red; border-radius: 10px 10px 3px green, 15px 15px 3px red;">
            This is example of box shadow
        </div>
    </body>
</html>
```



### Float

- float: left
- float: right
- float: none

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Box shadow</title>
    </head>
    <body>
        <div style="border: 10px solid red; width: 45%; float: left;">
            This is example of box shadow
        </div>
        <div style="border: 10px solid red; width: 45%; float: right;">
            This is example of box shadow
        </div>
    </body>
</html>
```

