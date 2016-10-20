Animation with Noah
Ref: Noah’s Blocks https://bl.ocks.org/veltman

Dashed Lines
Dash Animation
https://bl.ocks.org/veltman/e23c36540c7e89f774d5c663090933c7

Seamless Animated Dash
https://bl.ocks.org/veltman/fa74a3aff8497e970454bb064cf8dfd1

(Eventually it won’t be needed with the new SVG version coming: https://www.w3.org/TR/svg-strokes/#StrokeDashadjustProperty)

Animating along a Line
https://bl.ocks.org/veltman/1d6da36a626dd265f700d5a583e74e94

This trick could be useful for animating almost anything.

Using the same technique we have the self-drawing arrow demo.

We can use .attr(‘stroke-dasharray’, ‘20, 10’), where these numbers represent ranges of ‘drawing’ and ‘white space’ on the line.

Using ‘stroke-dasharray’ we can use tricks like in Animated subpath
Also we can see it on the Swoopy Arrows block
Or on top of a map in the Swoopy US Map

We have a CSS animation example on the Mystery Box demo

Transitioning Shapes
We can transition shapes like he does on maps on the Redistricting demo.
The problem when transitioning tabs is when the current and future shape don’t have the same number of points. 

In order to overcome this issue:
Add points to the shape that has less points until you equalize the number of that both the final shape and the current shape have
To decide where to add points, loop through each index you could add a point to the first shape, work out the sum of squares of distance that they’d have to travel, pick the minimal distance
Animate

(Noah uses mapshaper to simplify shapes in a pre-processing step)

We can see another demo on the Smoother Polygon transitions demo

On Jigsaw Morphing we see how to tween between a single polygon and multiple polygons. Another example is the Electoral Cartograms.

In the performance side, we need to know with which other elements our animation will be competing for CPU/GPU resources on the page.



