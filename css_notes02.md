## CSS Notes 2: Box Model

## 1. What is the CSS Box Model?
The CSS Box Model is a container that wraps around every HTML element.

+---------------------------+
|        Margin             |
|  +--------------------+   |
|  |    Border           |  |
|  |  +--------------+   |  |
|  |  |  Padding     |   |  |
|  |  | +---------+  |   |  |
|  |  | | Content |  |   |  |
|  |  | +---------+  |   |  |
|  |  +--------------+   |  |
|  +--------------------+   |
+---------------------------+


## Parts of box model

Part	             Description
Content	      The actual text or image in the box
Padding	      Space between content and border
Border	      The line surrounding the padding (and content)
Margin	      Space outside the border, creates distance between elements


## 3. CSS Properties
Content
Comes from the element itself: text, image, etc.

Padding

div {
  padding: 20px; /* Space inside the border */
}
Shorthand: padding: top right bottom left;

padding: 10px 15px 20px 25px;
Border

div {
  border: 2px solid black;
}
Border style types: solid, dashed, dotted, double, none

Margin

div {
  margin: 30px;
}
Shorthand: margin: top right bottom left;


margin: 10px 15px 20px 25px;


## 4. Box-Sizing Property
By default, padding and border add to the total width/height of an element.


div {
  box-sizing: border-box;
}
content-box (default): width = content only

border-box: width includes padding and border

## 5. Visual Example

.box {
  width: 200px;
  padding: 20px;
  border: 2px solid red;
  margin: 30px;
}
Total Width Calculation:


width = 200px (content)
+ padding: 20px * 2 = 40px
+ border: 2px * 2 = 4px
Total: 244px
If you use:

box-sizing: border-box;
Then total stays at 200px.

## 6. Developer Tools Tip
Use Inspect Element → Hover over elements to see:

Margin (orange)

Border (yellow)

Padding (green)

Content (blue)

## 7. Use-Cases
Padding: To create space inside the box.

Margin: To create space between boxes.

Border: To make boxes stand out.

Box-Sizing: To control box size calculations.