# css notes 05

## 🎨 1. CSS Transition 
Smooth change between property values.

Works with properties like color, background, transform, opacity, etc.

Syntax:

selector {
  transition: property duration timing-function delay;
}
Example:


.box {
  transition: background-color 0.5s ease;
}

.box:hover {
  background-color: blue;
}
Tip:
You can also use all to transition multiple properties.

transition: all 0.3s ease;


## 🎨 2. CSS Transform 
Used to visually manipulate elements (rotate, scale, move, skew).

🔄 a) Rotate (4:59:26)

.box {
  transform: rotate(45deg);
}
Positive = clockwise, Negative = counter-clockwise.

📏 b) Scale (5:05:17)

.box {
  transform: scale(1.5); /* 1.5 times bigger */
}
scaleX() or scaleY() for specific axes.

🚚 c) Translate (5:09:00)

.box {
  transform: translate(50px, 100px);
}
Moves the element along X and Y axes.

🪞 d) Skew (5:12:34)

.box {
  transform: skew(20deg, 10deg);
}
Distorts the shape along X and Y axes.

Tip:
You can combine transforms!

transform: rotate(30deg) scale(1.2) translate(20px, 30px);


## 🎨 3. CSS Animation 
Used for creating complex animations.

Steps:

Define keyframes.

Apply animation property.

Example:

@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

.box {
  animation: example 3s ease infinite;
}


## 🎨 4. Animation Shorthand 
Full shorthand:

animation: name duration timing-function delay iteration-count direction fill-mode;
Example:

animation: slide 2s linear 0s infinite alternate;
Tip:

infinite = loop forever

alternate = reverse on every loop

ease, linear, ease-in, ease-out = speed curve


## 🎨 5. Animation with % Keyframes 
Use percentages for multiple stages!

Example:

@keyframes colorChange {
  0% { background-color: red; }
  50% { background-color: yellow; }
  100% { background-color: green; }
}

.box {
  animation: colorChange 4s infinite;
}


