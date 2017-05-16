# Pulling a polygon out of a hat - Noah Veltman

[Youtube Link](https://www.youtube.com/watch?v=PLc1y-gim_0)

- North carolina gerrymandering
- Animate transition between district lines from 2011 to 2016
- Initial transitions looks picasso-esque
  - Items jumps around too much
- InbeTweening - in between frames in animation
- Color transitioning - many different ways of approaching
- Noah Duncan - horse to chair
- The Correspondence Problem - or the Orange and Apples problem
- Undercover hexagon is the square that adds two points
  - Smoother animation
- Also helps with curves, by decompositions
- Order of the points matter - test every starting point until you get it right
1. Add dummy points
2. Pick a starting point
- d3-interpolate-path: animate between lines

## The Quest
- What in academia has this solution?
- Prior art
- Beier-neely morphing algorithm
  - Not automatic!
- 2D Polygon Morphing using the Extended Gaussian Image - http://web.mit.edu/manoli/ecimorph/www/ecimorph.html
  - Not any two shapes! polygons only...
- The Trajectory Problem
- Procrustes - Greek myth origin - for statistical thinking for stretching
- Procrustean - rotate, translate, then morphing as separate steps
  - Not looking natural

- Shape to shape = good
- multi-polygons != good
- How about a technique where you can throw multi-polygon shapes?
- How do you turn California into Hawaii

1. Draw a grid
  - Voronoid diagram
2. Assign starter cells
3. Assign neighbors
  - Like a game of risk - weighted to give more shape to larger polygons
4. Merge and clip

- Triangulation - carve from the inside out
1. Triangulate
2. Merge two neighbors, repeat 

## The cut
- Incision in your shape
- pushing the hole out

## The wink
- Blink it out of existence

## Closing quote
> The solution presented here is a heuristic whose justification lies in the fact that it generally seems to work rather well
> Computer Graphics 1993
> Sederberg, Wany, and Mu
> 2D shape blending: An intrinsic solution to the vertex path problem
