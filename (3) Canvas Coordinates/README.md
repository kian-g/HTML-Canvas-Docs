- [Draw a Line](#draw-a-line)
  * [Example](#example)
- [Draw a Circle](#draw-a-circle)
  * [Example](#example-1)
___
The HTML canvas is a two-dimensional grid.

The upper-left corner of the canvas has the coordinates (0,0)

In the previous chapter, you saw this method used: fillRect(0,0,150,75).

This means: Start at the upper-left corner (0,0) and draw a 150x75 pixels rectangle.

# Draw a Line
To draw a straight line on a canvas, use the following methods:
- moveTo(x,y) - defines the starting point of the line
- lineTo(x,y) - defines the ending point of the line
To actually draw the line, you must use one of the "ink" methods, like stroke().
## Example
Define a starting point in position (0,0), and an ending point in position (200,100). Then use the stroke() method to actually draw the line:
```js
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.moveTo(0, 0);
ctx.lineTo(200, 100);
ctx.stroke();
```

# Draw a Circle
To draw a circle on a canvas, use the following methods:
- beginPath() - begins a path
- arc(x,y,r,startangle,endangle) - creates an arc/curve. To create a circle with arc(): Set start angle to 0 and end angle to 2\*Math.PI. The x and y parameters define the x- and y-coordinates of the center of the circle. The r parameter defines the radius of the circle.
## Example
Define a circle with the arc() method. Then use the stroke() method to actually draw the circle:
```js
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
```
