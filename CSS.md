# **CSS**

## **Selectors**

### **The CSS element Selector**

```
p {
  text-align: center;
  color: red;
}
```
### **The CSS id Selector**

```
#para1 {
  text-align: center;
  color: red;
}
```

### **The CSS class Selector**

```
.center {
  text-align: center;
  color: red;
}
```

*In this example only <p> elements with class="center" will be red and center-aligned:*

```
p.center {
  text-align: center;
  color: red;
}
```

### **The CSS Universal Selector**
```
* {
  text-align: center;
  color: blue;
}
```

*To group selectors, separate each selector with a comma.*

## **How to add CSS?**

### **Inline CSS**

```
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```

## **Comments**
```
/* This is a single-line comment */
p {
  color: red;
}
```

## **Colors**

### **Background Color**
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p>
```

### **CSS Text Color**
```
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>
```

## **Background**

### **background-color:**
```
div {
  background-color: green;
  opacity: 0.3;
}
```
![Текст описания](file:///Users/saprykinadara/Desktop/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202023-06-07%20%D0%B2%2014.29.16.png)

### **background-image**
```
body {
  background-image: url("paper.gif");
}
```

### **background-repeat**

```
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}
```
*horizontal repeating*

```
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-y;
}
```
*vertical repeating*

### **background-position**
```
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```

### **background-attachment**
The background-attachment property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page):
```
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed (scroll);
}
```
```
body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
```
Use the shorthand property to set the background properties in one declaration.

## **Borders**

### **Border-style**
```
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
```

![Текст описания](border.png)

### **Border-Width**
```
p.two {
  border-style: solid;
  border-width: medium;
}
```
### **Border-Color**
```
p.one {
  border-style: solid;
  border-color: red;
}
```
### **Border-Radius**
The border-radius property is used to add rounded borders to an element:
```
p {
  border: 2px solid red;
  border-radius: 5px;
}
```
## **Margins**
Margin are used to creat space aroun elements outside of borders
top - right - bottom - left
```
p {
  margin: 25px 50px 75px 100px;
}
```
## **Padding**
Padding is used to create space around an element's content, inside of borders.
```
div {
  padding: 25px 50px 75px 100px;
}
```
top - right - bottom - left
### **Padding and element width**
```
div {
  width: 300px;
  padding: 25px;
}
```
*Here, the <div> element is given a width of 300px. However, the actual width of the <div> element will be 350px (300px + 25px of left padding + 25px of right padding):*

```
div {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
}
```
*Use the box-sizing property to keep the width at 300px, no matter the amount of padding:*

## **Height, width and max-width**
### **Setting max-width**
The problem with the <div> above occurs when the browser window is smaller than the width of the element (500px). The browser then adds a horizontal scrollbar to the page.

Using max-width instead, in this situation, will improve the browser's handling of small windows.

## **Box Model**
The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:

The total height of an element should be calculated like this:

Total element height = height + top padding + bottom padding + top border + bottom border + top margin + bottom margin

## **Outline**
An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element "stand out".

### **Style**
- dotted - Defines a dotted outline
- dashed - Defines a dashed outline
- solid - Defines a solid outline
- double - Defines a double outline
- groove - Defines a 3D grooved outline
- ridge - Defines a 3D ridged outline
- inset - Defines a 3D inset outline
- outset - Defines a 3D outset outline
- none - Defines no outline
- hidden - Defines a hidden outline

*Outline also can have a width and a color.*

### **Shorthand property**
```
p {
    outline: dashed, 5px, yellow;
}
```
### **Outline offset**
This property adds space between an outline and the border of an element. 

## **Text**
```
p {
    color: black;
    text-align: center;
    text-align-last: center;           
    vertical-align: text-top, text-bottom, sub, super, baseline;
    text-decoration-line: overline, line-through, underline;
    text-decoration-color: black;
    text-decoration-style: double, solid, dotted, dashed, wavy;
    text-decoration-thickness: 5px;
    text-transform: capitalize, lowercase, uppercase;
    text-indent: 50px;
    letter-spacing: 5px;
    word-spacing: 10px;
    line-height: 0.8;
    text-shadow: 2px 2px red;
}
```
## **Fonts**
```
p {
    font-family: Arial;
    font-style: italic, oblique, normal;
    font-weight: bold, normal, 700px;
    font-size: 40px;
    font: Arial italic bold 40px;
}
```
## **Icons**
### **Bootstrap Icons**
```
<head>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
```
### **Google Icons**
```
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
```
## **Links**
The four links states are:
- a:link - a normal, unvisited link
- a:visited - a link the user has visited 
- a:hover - a link when the user mouses over it
- a:active - a link the moment it is clicked

## **Lists**
### **List Style**
List-style considers only markers of the list.
```
ul {
    list-style-type: circle, square, upper-poman, lower-alpha;
    list-style-image: url(image.png);
    list-style-position: outside, inside;
}
```




