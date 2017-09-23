# Taking Care of Gifness

## Rendering outside of the browser

Use Cases

- Portability
- Performance
- Code once, generate many
- Work in JS instead of animation software

Own goals: Develop image for making negative
- Needs: halftones, guidelines, conversion from color to grayscale

Techniques:
1. Manual Capture
1. Helper Code
1. Server Side
1. Headless Browser

[Slides for reference](http://slides.com/veltman/d3unconf#/)

Render loop - Canvas - must specify every detail. can render any frame
- Disco globe - must draw on every rotation (every 20ms)

With D3.transition()
- No frame-seeking. Uses timing and chaining

Gif.js
Gifsicle - cli tool

ffmpeg
- tmcw animation canvas
- github.com/tmcw

greensock animations

