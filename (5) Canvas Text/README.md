- [Drawing Text on the Canvas](#drawing-text-on-the-canvas)
- [Using fillText()](#using-filltext)
  * [Example](#example)
- [Using strokeText()](#using-stroketext)
  * [Example](#example-1)
- [Add Color and Center Text](#add-color-and-center-text)
  * [Example](#example-2)

# Drawing Text on the Canvas
To draw text on a canvas, the most important property and methods are:
- font - defines the font properties for the text
- fillText(text,x,y) - draws "filled" text on the canvas
- strokeText(text,x,y) - draws text on the canvas (no fill)
# Using fillText()
## Example
Set font to 30px "Arial" and write a filled text on the canvas:
```js
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
```

# Using strokeText()
## Example
Set font to 30px "Arial" and write a text, with no fill, on the canvas:
```js
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World", 10, 50);
```

# Add Color and Center Text
## Example
Set font to 30px "Comic Sans MS" and write a filled red text in the center of the canvas:
```js
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Comic Sans MS";
ctx.fillStyle = "red";
ctx.textAlign = "center";
ctx.fillText("Hello World", canvas.width/2, canvas.height/2);
```
