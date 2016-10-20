d3.unconf 2016
Session 2: 1:30pm
Library
Modular & Reusable
Motivations for Modular Code
Much faster to debug files when they are small and code is not duplicated
Distributed development benefits from modular code
Easier to work with a web development team using different tools
Tools & Apps
Build Systems
Rollup: http://rollupjs.org/
Webpack: https://webpack.github.io/
Wrapping
Piper.js
Piper.js - Piper.js is a simple pipeline pattern to build charts. It's a way to modularize tiny pieces of D3 code and assemble them.
Piper.js Pipeline - https://github.com/biovisualize/piper.js/blob/master/src/chart-pipeline.js
Able to talk down, but not talk up
Each module declares what it needs. Configs have defaults and can override
And there's a branch using Rollup https://github.com/biovisualize/piper.js/tree/rollup
D3 Kit
https://github.com/twitter/d3kit
Scaffolding or making reusable charts. 
Support both SVG, Canvas
Set up component, handle resize and let user set data, then get out of the way to let you implement the component the way you want (mostly copy and modify from blocks to change width to this.getInnerWidth() and height to this.getInnerHeight()). 
https://github.com/twitter/d3kit/tree/v3
https://github.com/kristw/react-d3kit

How do we wrap charts? Post them to Slack Channel #unconf
Koto
Next version of d3 Charts
https://github.com/kotojs/kotojs
http://kotojs.org/
Problems / Constraints
Roll-up ES6 hooks
Using babelrc config for globals like lodash
https://gist.github.com/kristw/302a6bac31102972867b851fd76ccc89

What else should be reusable / modular?
D3 behavior: Physics engines, Throw
Numeral Sort

Using other platforms
Cygwin - https://www.cygwin.com/

Event Handling
Simple API to pass multiple functions to a particular element
Binding new event listeners on SVG
Teardown of event listeners on SVG

StateMachine
https://github.com/jakesgordon/javascript-state-machine 
Links / Resources
D3.js —Use it as Custom modular Bundle Now!! - https://medium.com/@richavyas/d3-js-the-custom-modular-bundle-now-bebd6f25bc8b
D3-BoundingBox - https://github.com/lucasb-eyer/d3-boundingbox
D3-jetpack-module - https://github.com/1wheel/d3-jetpack-module

