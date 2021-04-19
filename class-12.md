charts:
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly,

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script


he <canvas> element has only two attributes, width and height.

There are three functions that draw rectangles on the canvas:

fillRect(x, y, width, height) Draws a filled rectangle
strokeRect(x, y, width, height) Draws a rectangular outline.
clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.
The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth]) Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
by developer.mozilla.org