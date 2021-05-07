- [What is HTML Canvas?](#what-is-html-canvas)
- [Browser Support](#browser-support)
- [HTML Canvas Can Draw Text](#html-canvas-can-draw-text)
- [HTML Canvas Can Draw Graphics](#html-canvas-can-draw-graphics)
- [HTML Canvas Can be Animated](#html-canvas-can-be-animated)
- [HTML Canvas Can be Interactive](#html-canvas-can-be-interactive)
- [HTML Canvas Can be Used in Games](#html-canvas-can-be-used-in-games)
- [Canvas Example](#canvas-example)

The HTML <canvas> element is used to draw graphics on a web page.

The graphic above is created with <canvas>.

It shows four elements: a red rectangle, a gradient rectangle, a multicolor rectangle, and a multicolor text.

# What is HTML Canvas?
The HTML <canvas> element is used to draw graphics, on the fly, via scripting (usually JavaScript).

The <canvas> element is only a container for graphics. You must use a script to actually draw the graphics.

Canvas has several methods for drawing paths, boxes, circles, text, and adding images.

# Browser Support
The numbers in the table specify the first browser version that fully supports the <canvas> element.
| Element | Chrome | Edge | Firefox | Safari | Opera |
| ------- | ------ | ---- | ------- | ------ | ----- |
| \<canvas> | 4.0 | 9.0 | 2.0 | 3.1 | 9.0 |

# HTML Canvas Can Draw Text
Canvas can draw colorful text, with or without animation.

# HTML Canvas Can Draw Graphics
Canvas has great features for graphical data presentation with an imagery of graphs and charts.

# HTML Canvas Can be Animated
Canvas objects can move. Everything is possible: from simple bouncing balls to complex animations.

# HTML Canvas Can be Interactive
Canvas can respond to JavaScript events.

Canvas can respond to any user action (key clicks, mouse clicks, button clicks, finger movement).

# HTML Canvas Can be Used in Games
Canvas' methods for animations, offer a lot of possibilities for HTML gaming applications.

# Canvas Example
In HTML, a \<canvas> element looks like this:
```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```
The \<canvas> element must have an id attribute so it can be referred to by JavaScript.

The width and height attribute is necessary to define the size of the canvas.

**Tip:** You can have multiple \<canvas> elements on one HTML page.
```
By default, the <canvas> element has no border and no content.
```
To add a border, use a style attribute:
```html
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>
```
