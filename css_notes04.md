# CSS Notes - Part 4


## Flexbox
Flexbox = Flexible Box Layout.

Used to design flexible, responsive layout structures without using float or positioning.

Flexbox layouts work on one dimension at a time — row or column.


## Flex Model
Flexbox has 2 main parts:

Flex Container (parent element)

Flex Items (child elements)


## Flex Container Properties


1. display: flex;
Makes an element a flex container.

Example:

.container {
  display: flex;
}


2. flex-direction
Defines the direction of flex items.

Values:

row (default) → left to right

row-reverse → right to left

column → top to bottom

column-reverse → bottom to top

Example:

.container {
  flex-direction: row;
}


3. justify-content

Aligns items horizontally (main axis).

Values:

flex-start (default)

flex-end

center

space-between

space-around

space-evenly

Example:

.container {
  justify-content: space-between;
}


4. flex-wrap
Controls if items should wrap or stay in one line.

Values:

nowrap (default)

wrap

wrap-reverse

Example:

.container {
  flex-wrap: wrap;
}


5. align-items
Aligns items vertically (cross-axis).

Values:

stretch (default)

flex-start

flex-end

center

baseline

Example:

.container {
  align-items: center;
}


6. align-content
Aligns multiple lines of items when flex-wrap is used.

Values:

flex-start

flex-end

center

space-between

space-around

stretch (default)

Example:

.container {
  align-content: center;
}


## Flex Item Properties

1. flex-grow
Defines how much an item will grow relative to others.

Example:

.item {
  flex-grow: 2;
}

2. flex-shrink
Defines how much an item will shrink if space is tight.

Example:

.item {
  flex-shrink: 1;
}

3. flex-basis
Defines the initial size of an item before space is distributed.

Example:

.item {
  flex-basis: 100px;
}

4. flex
Shorthand for:

flex: grow shrink basis;
Example:

.item {
  flex: 1 1 100px;
}

5. align-self
Allows an item to override the container’s align-items.

Values:

auto (default)

flex-start

flex-end

center

baseline

stretch

Example:

.item {
  align-self: flex-end;
}


## Media Queries

Media queries = Make websites responsive by applying CSS rules based on device features like screen width.

Syntax:


@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
Common examples:

/* Mobile phones */
@media (max-width: 480px) { ... }

/* Tablets */
@media (min-width: 481px) and (max-width: 768px) { ... }

/* Desktops */
@media (min-width: 769px) { ... }


## Quick Summary Table
          
          Property                                                    	Use
 
        display: flex;	                                       Makes container flex
        flex-direction	                                       Sets direction (row/column)
        justify-content	                                       Horizontal alignment
        flex-wrap	                                           Wrap items or not
        align-items	                                           Vertical alignment
        align-content	                                       Align multiple lines
        flex-grow	                                           Grow ratio of item
        flex-shrink                                            Shrink ratio of item
        flex-basis	                                           Initial size of item
        flex	                                               Shorthand for grow, shrink, basis
        align-self	                                           Individual item alignment


        