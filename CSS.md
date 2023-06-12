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
