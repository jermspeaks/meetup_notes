# d3.unconf 2016

## Session 1: 11am

Library

## d3.js v4

Changes in D3 V4.0 https://github.com/d3/d3/blob/master/CHANGES.md  
D3 V4 - What’s New? https://iros.github.io/d3-v4-whats-new/

Possible Topics to Explore in other unconf sessions

How to integrate with Webpack or other bundlers?
Object.assign(d3, d3-submodule)?  Seems hacky…

New general update pattern: d3. merge()

Intro to canvas:  Interaction, animation/tweening?

Evolving practices: styling CSS/JS?

How to live together d3.v3 and d3.d4? Any practical examples?

Can anyone  share a link to the slide deck with the venn diagrams shown earlier?

Discussion: What are the coolest parts about d3 v4?
Canvas
Canvas rendering: Starting v4, many of the rendering helpers now have a new context method that lets you pass in a Canvas context to render to. (from Irene Ros’ slide deck referenced above)

Simulation.find -- will give you the closest canvas node to what is clicked on.  Example
Canvas mouse events example (painting with colors, master layer for mouse events).  You can also do voronoi, manually calculating X&Y.  css-pointer events (weird, broke on safari).
In canvas, enter() exit() is handled by an automatic clearing canvas instead of the functions themselves. 
Force Layout
In v4, you specify all of the forces that you want (some defaults are supplied) and mix and match your custom forces with the default ones.   See the code in Elijah Meeks’ block called d3-bboxCollide

Force options in action

Hierarchy Layout
If your data is not already in a hierarchical format and is instead in tabular format, you can use d3.stratify to make your data hierarchical

