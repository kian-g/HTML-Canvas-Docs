- [Draw on the Canvas With JavaScript](#draw-on-the-canvas-with-javascript)
  * [Example](#example)
- [Step 1: Find the Canvas Element](#step-1--find-the-canvas-element)
- [Step 2: Create a Drawing Object](#step-2--create-a-drawing-object)
- [Step 3: Draw on the Canvas](#step-3--draw-on-the-canvas)
___
# Draw on the Canvas With JavaScript
All drawing on the HTML canvas must be done with JavaScript:
## Example
```html
<script>
  var canvas = document.getElementById("myCanvas");
  var ctx = canvas.getContext("2d");
  ctx.fillStyle = "#FF0000";
  ctx.fillRect(0, 0, 150, 75);
</script>
```

# Step 1: Find the Canvas Element
First of all, you must find the <canvas> element.

This is done by using the HTML DOM method getElementById():
```js
var canvas = document.getElementById("myCanvas");
```

# Step 2: Create a Drawing Object
Secondly, you need a drawing object for the canvas.

The getContext() is a built-in HTML object, with properties and methods for drawing:
```js
var ctx = canvas.getContext("2d");
```

# Step 3: Draw on the Canvas
Finally, you can draw on the canvas.

Set the fill style of the drawing object to the color red:
```js
ctx.fillStyle = "#FF0000";
```
The fillStyle property can be a CSS color, a gradient, or a pattern. The default fillStyle is black.

The fillRect(*x, y, width, height*) method draws a rectangle, filled with the fill style, on the canvas:
```js
ctx.fillRect(0, 0, 150, 75);
```
