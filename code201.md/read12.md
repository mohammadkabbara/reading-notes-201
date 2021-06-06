# Chart.js

**Creating a Chart**

It's easy to get started with Chart.js. All that's required is the script included in your page along with a single <canvas node to render the chart.

---------

**Fallback content**


The canvas> element differs from an img> tag in that, like for video>, audio>, or picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

Providing fallback content is very straightforward: just insert the alternate content inside the canvas> element. Browsers that don't support canvas> will ignore the container and render the fallback content inside it. Browsers that do support canvas> will ignore the content inside the container, and just render the canvas normally.


**Checking for support**

The fallback content is displayed in browsers which do not support canvas>. Scripts can also check for support programmatically by testing for the presence of the getContext() method. Our code snippet from above becomes something like this:

var canvas = document.getElementById('tutorial');


if (canvas.getContext) {

  var ctx = canvas.getContext('2d');

  // drawing code here

} else {

  // canvas-unsupported code here
}

# Drawing paths

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:


First, you create the path.

Then you use drawing commands to draw into the path.

Once the path has been created, you can stroke or fill the path to render it.

Here are the functions used to perform these steps:


**beginPath()**

Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

**Path methods**

Methods to set different paths for objects.

**closePath()**

Adds a straight line to the path, going to the start of the current sub-path.

**stroke()**

Draws the shape by stroking its outline.

**fill()**

Draws a solid shape by filling the path's content area.

*The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.*


# Moving the pen


One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.

**moveTo(x, y)**

Moves the pen to the coordinates specified by x and y.

When the canvas is initialized or beginPath() is called, you typically will want to use the moveTo() function to place the starting point somewhere else. We could also use moveTo() to draw unconnected paths


# A lineCap example

The lineCap property determines how the end points of every line are drawn. There are three possible values for this property and those are: butt, round and square. By default this property is set to butt.

**butt**

The ends of lines are squared off at the endpoints.

**round**

The ends of lines are rounded.

**square**

The ends of lines are squared off by adding a box with an equal width and half the height of the line's thickness.

# Styling text

In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:


**font = value**

The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

**textAlign = value**

Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

**textBaseline = value**

Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

**direction = value**

Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

These properties might be familiar to you, if you have worked with CSS before.


