# CSS Notes 1: Basics (Colors & Fonts)

## 1. Selectors

/* Target elements */
p { }        /* Paragraph */
h1 { }       /* Heading 1 */
.className { }  /* Class */
#idName { }     /* ID */


# 2. Colors

/* Color names */
p {
  color: red;
}

/* HEX codes */
h1 {
  color: #3498db;  /* Light blue */
}

/* RGB */
div {
  color: rgb(255, 0, 0);  /* Red */
}

/* Background color */
body {
  background-color: #f0f0f0;
}


# 3. Fonts

/* Font family */
body {
  font-family: Arial, sans-serif;
}

/* Font size */
p {
  font-size: 16px;
}

/* Font weight */
h1 {
  font-weight: bold;
}

/* Font style */
em {
  font-style: italic;
}


## 4. Text Styling

/* Text alignment */
h1 {
  text-align: center;
}

/* Text decoration */
a {
  text-decoration: none;
}

/* Text transform */
p {
  text-transform: uppercase;
}



## 1. Types of CSS
Inline CSS

<p style="color: red;">This is inline CSS</p>
Internal CSS


<head>
  <style>
    p { color: blue; }
  </style>
</head>
External CSS


<head>
  <link rel="stylesheet" href="style.css">
</head>


## 2. CSS Selectors
Selector Type	                    Example	                  Description
Element Selector	                p { }	             Targets all <p> tags
Class Selector	                .className { }	         Targets elements with class="className"
ID Selector	#idName                  { }	             Targets element with id="idName"
Universal Selector	               * { }	             Targets all elements
Grouping Selector	              h1, p { }	             Applies same style to multiple elements
Descendant Selector	               div p { }	         Targets <p> inside <div>


## 3. Fonts

/* Font family */
body {
  font-family: Arial, Verdana, sans-serif;
}

/* Font size */
p {
  font-size: 18px;
}

/* Font weight */
h1 {
  font-weight: bold;
}

/* Font style */
em {
  font-style: italic;
}


## 4. Colors

/* Named color */
h1 {
  color: green;
}

/* HEX color */
p {
  color: #e74c3c;
}

/* RGB */
div {
  color: rgb(52, 152, 219);
}

/* Background color */
body {
  background-color: #f4f4f4;
}


## 5. Commands / Properties (Basics)
Property	                       Example	                             Description
color	                          color: red;	                          Text color
background-color	        background-color: yellow;	               Background color
font-size	                   font-size: 16px;	                       Size of the text
font-family	                   font-family: Arial;	                       Text font
text-align	                  text-align: center;	                       Align text
font-weight	                    font-weight: bold;	                       Bold text
text-decoration	               text-decoration: none;	         Remove underline from links


## 6. Development Tools
Browser Developer Tools (Inspect Element):

Right-click on any webpage → Inspect

Check and edit CSS live.

VS Code Extensions:

Live Server — For real-time preview.

Prettier — For formatting CSS.

Color Highlight — To preview CSS colors in the code.

Online Tools:

CSS Gradient Generator

Google Fonts

Color Picker

