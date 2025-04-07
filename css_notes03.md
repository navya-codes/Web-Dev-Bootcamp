# CSS Notes 

## 1. Units in CSS
CSS uses units to define sizes (like width, height, margin, padding, font size, etc.)

Absolute units (Fixed size):

px (pixels)

cm, mm, in (centimeter, millimeter, inch)

pt, pc (points, picas — mostly for print)

Relative units (Responsive, better for modern design):

% (percentage)

em, rem

vw, vh

vmin, vmax

## 2. Percentage (%)
Based on the parent element’s size.

Example:

div {
  width: 50%; /* 50% of the parent container */
}


## 3. em
Relative to the font-size of the parent.

Example:


body {
  font-size: 16px;
}
p {
  font-size: 2em; /* 2 × 16px = 32px */
}


## 4. rem (Root em)
Relative to the root element (html) font size.

Example:


html {
  font-size: 16px;
}
p {
  font-size: 2rem; /* 2 × 16px = 32px */
}


## 5. vh & vw
vh = viewport height (1vh = 1% of the viewport height)

vw = viewport width (1vw = 1% of the viewport width)

Example:


div {
  width: 50vw; /* 50% of the viewport width */
  height: 50vh; /* 50% of the viewport height */
}


## 6. Position in CSS
Static (default)
Elements follow normal document flow.


div {
  position: static;
}
Relative
Positioned relative to itself (its normal position).


div {
  position: relative;
  top: 10px; /* Moves down by 10px from its normal position */
}
Absolute
Positioned relative to the nearest positioned ancestor.

If no positioned ancestor, it uses the <html> document.


div {
  position: absolute;
  top: 20px;
  left: 30px;
}
Fixed
Positioned relative to the viewport (doesn’t move when scrolling).


div {
  position: fixed;
  top: 0;
  right: 0;
}
Sticky
Acts like relative until a certain scroll point, then behaves like fixed.


div {
  position: sticky;
  top: 10px;
}

## 7. Z-Index
Controls the stacking order of overlapping elements.

Higher z-index = in front.


div {
  position: absolute;
  z-index: 10;
}
Note: z-index works only on positioned elements (relative, absolute, fixed, sticky).

## 8. Background Image
Adds an image in the background of an element.


div {
  background-image: url('image.jpg');
}

## 9. Background Size
Controls the size of the background image.

Options:

cover — fills the container (might crop).

contain — fits the image entirely (might leave space).

Example:


div {
  background-image: url('image.jpg');
  background-size: cover;
}


## 10. Background Repeat
Controls if the background image repeats.

Options:

repeat (default) — repeats both vertically and horizontally.

no-repeat — shows the image only once.

repeat-x — repeats horizontally.

repeat-y — repeats vertically.

Example:


div {
  background-image: url('image.jpg');
  background-repeat: no-repeat;
}
Summary Table
Property	                                             Description
%	                                            Percentage of parent container
em	                                            Relative to parent font-size
rem                                         	Relative to root font-size
vh/vw	                                        Viewport height/width percentage
position: static	                            Default position
position: relative	                            Relative to normal position
position: absolute	                            Relative to nearest positioned ancestor
position: fixed	                                Fixed to viewport
position: sticky                            	Scroll-dependent fixed position


z-index	Stack order of elements

background-image	                            Set background image
background-size	                                Size of background image
background-repeat	                            Repeat behavior of background image