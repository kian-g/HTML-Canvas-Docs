- [Using createLinearGradient()](#using-createlineargradient)
  * [Example](#example)
- [Using createRadialGradient():](#using-createradialgradient)
  * [Example](#example-1)

Gradients can be used to fill rectangles, circles, lines, text, etc. Shapes on the canvas are not limited to solid colors.

There are two different types of gradients:

createLinearGradient(x,y,x1,y1) - creates a linear gradient
createRadialGradient(x,y,r,x1,y1,r1) - creates a radial/circular gradient
Once we have a gradient object, we must add two or more color stops.

The addColorStop() method specifies the color stops, and its position along the gradient. Gradient positions can be anywhere between 0 to 1.

To use the gradient, set the fillStyle or strokeStyle property to the gradient, then draw the shape (rectangle, text, or a line).

# Using createLinearGradient()
## Example
Create a linear gradient. Fill rectangle with the gradient:
```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createLinearGradient(0, 0, 200, 0);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
```

# Using createRadialGradient():
## Example
Create a radial/circular gradient. Fill rectangle with the gradient:
```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
```
