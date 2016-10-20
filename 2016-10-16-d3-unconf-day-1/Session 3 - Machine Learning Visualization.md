d3.unconf 2016
Session 3: 2:30pm
Alcatraz
Machine Learning Visualization

Tony - 2 kinds of visualizations he makes:
more for internal audience, visualizing for data scientists and domain experts: stuff like residual plots (vis as tools)
more for external audience, non-data scientists. e.g. r2d3
want to explain the intuition, not the math (another good example is Tensorflow Playground from Google: http://playground.tensorflow.org/) 

Some inbetween: how to convey probabilistic nuance to consumers of a result
conveying confidence to person viewing result
Jessica Hullman - Visual Uncertainty Experience
Trust & statistics - how to communicate how much one should trust

Explorable explanation of t-SNE - visualization plus article full of examples (small multiples that you can click on) to help understanding:
http://distill.pub/2016/misread-tsne/ 

How to encourage clicking/interacting?
Victor made GIFs to show possible interactions
http://setosa.io/ev/ordinary-least-squares-regression/
also had more subtle pulsing of interactive elements
http://setosa.io/ev/principal-component-analysis/
Tony wants to link everything to scroll so there is no discoverability issue
A movie you play through by scrolling. you control the pace and can rewind easily

NYTimes fades in cursor to brute force show user that something is interactive

Graceful degradation - if it works without the interaction thats even better

Visualizing parameter space explorations - showing history of runs
some algorithms lend themselves better to animation, stepping
non-deterministic algorithms might be a little challenging, small multiples can help

this is the technique that we are using
these are the problems it faces
dirichlet processes - http://people.csail.mit.edu/tbroderick/present.html  -- specifically this http://people.csail.mit.edu/tbroderick/tutorial_2016_mlss_cadiz.html


how do you show 10 features? having more than a few important variables that need to be conveyed
visualizing higher-dimensions gets really confusing
dimensionality reduction
multiple scatterplots
bivariate heatmaps
LIME explanations https://github.com/marcotcr/lime
Font manifolds: http://vecg.cs.ucl.ac.uk/Projects/projects_fonts/projects_fonts.html
parallel coordinates: http://bl.ocks.org/enjalot/beed3e8491e29ad1b1f8347516a65fc9


Glyphs:
 http://www.math.yorku.ca/SCS/sugi/sugi16-paper.html
http://www.datasketch.es/july/code/shirley/
http://www.oecdbetterlifeindex.org/#/11131111111

Managing many things on the page?
How do you deal with a lot of stuff going on at once.
Tony - try not to show many things.
find a way to transition from one type of plot to another, keep consistency
Bryan - likes it when multiple things work together. especially when they are linked
especially if there is a relationship you want to explain
also depends on who the audience is - data density can be very valuable for experts/data scientists
how much do you put on the user to interact - sliders & controls vs. playable animations
can also combine to allow users to dig deeper into interactive
good example of keeping consistency:
http://www.nytimes.com/interactive/2012/02/13/us/politics/2013-budget-proposal-graphic.html

3 distinct things you may want to visualize with ML
your data - e.g. using tSNE for exploration
your algorithm - e.g. explaining how NNs or decision trees work
your output - e.g. explaining your predictions or models  to others in a way they can understand

exploring the model
http://oppositionscience.com/predict.fball.outcome/var.selection.html

showing relationships that aren’t necessarily correlations:
https://en.wikipedia.org/wiki/Anscombe%27s_quartet
https://en.wikipedia.org/wiki/Correlation_and_dependence

feature importance - very useful place to start
https://topepo.github.io/caret/variable-importance.html



