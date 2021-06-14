# Reading 201-12: Chart.js, Canvas API

## Animated charts with Chart.js
This article by Sara Viera (what a fantastic name) can be found [here.](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

This article is a tutorial to chart.js, a plugin which uses the html canvas funtion to draw pretty charts onto your page. Awesome!

I was all set to jump into their suggested demo, when I found out the (unsuprisingly) chart.js has changed in the last seven years and it cannot be carried out as written. Aw, shucks. Quick hits from the rest of the article:

- we are presumably going to need a link to a separate .js file for the plugin
- chart.js works within html `<canvas>` elements
- we then need a script to generate a chart object in the element with a method for the type of chart
- Chart has many methods within that help form the tables
- We then give an object to make the chart out of that includes labels, data, and style settings
- all of the needed information is in this delightful repository's documentation. 

## MDN Canvas API 1: Basic Usage
This MDN article can be found [here.](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

- canvas elements have 2 attributes for width and height, and rather need them if the drawing is going to be successful. 
- Some browsers do not support canvas, and will need a fallback. luckily canvas needs a closing tag but nothing inside, so simply place the fallback between the tags. 
- the canvas generates a blank field for a script to draw on. The script can access this via the getContext method.

## MDN Canvas API 2: Drawing Shapes with Canvas
This is a continuation form the above article

Canvas operates as a grid using coordinates based on it's size attributes, usually measured in pixels. Canvas has several built in methods to draw shapes, which are outlined in the article. 

The other way to draw with canvas is via paths. A path is comprised of a list of points that form a line or shape, which can then be interacted with via methods.
- `beginPath()`: creates a new path
- `closepath()`: add a straight line to the path 
- `stroke()`: draw the shape of the path
- `fill()`: draw solid shape from the area of the path

The article provides some sample code for drawing a triangle:
```Javascript
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }
}
```
here we beginPath, moveto the start of the triangle, lineto one corner, then the next, then fill to finish. 

for curved lines (arcs) we can use arc or arcTo rather than lineTo. arc and arcTo are a bit more involved:

arc(x, y, radius, startAngle, endAngle, counterclockwise); (from article)
arcTo(x1, y1, x2, y2, radius)

We either define a radius and point, or the more detailed components of arc. The article also discusses quadratic curve options, and methods for combining these techniques for more complex drawing functions. 

##  MDN Canvas API 3: Applying Styles and Colors

fillStyle and strokeStyle can be defined as properties of the canvas to control the colors used in the drawing. `globalAlpha = transparencyValue` can be used to set transparency. Canvas objects also have a variety of built in line styles and other styling via properties. 

## MDN Canvas API 4: Drawing Text

fillText and strokeText are both options within canvas for adding text to drawings. This article covers another list of properties that can be used to style the drawn text, including font, size, and other similar properties to what is available in CSS. 

[<<Return to Home](../README.md)