d3.unconf 2016
Session 4: 3:30pm
Boardroom
Clustering

Eric Socolofsky: I worked with clustering in v4 recently and was surprised to find there’s no module yet. Here’s what I ended up writing, which is partway toward being modular, in case it’s worth talking about today:

http://bl.ocks.org/ericsoco/cd0c38a20141e997e926592264067db3
https://bl.ocks.org/ericsoco/38b4f8b51ecf116e6fb0727d25687e8e
https://bl.ocks.org/ericsoco/c3fdb4c844a88101f606e9db08e66845

Follows the example set by other d3.v4-force modules, e.g.
https://github.com/d3/d3-force/blob/master/src/x.js


K-means clustering, explained using d3:
http://www.bytemuse.com/post/k-means-clustering-visualization/

K-means voronoi relaxation:
https://bl.ocks.org/alexmacy/3986db72dc4b81db8e788dd837ee6e3b 

Using clustering to create a new d3.js color scale that’s more sensitive to the underlying data:
https://medium.com/@dschnr/using-clustering-to-create-a-new-d3-js-color-scale-dec4ccd639d2
https://cran.r-project.org/web/packages/Ckmeans.1d.dp/

Discussion of various methods for generating color scales, including Jenks Natural Breaks:
http://roadtolarissa.com/coloring-maps/

Finding the K in K-means clustering:
https://datasciencelab.wordpress.com/2013/12/27/finding-the-k-in-k-means-clustering/
https://datasciencelab.wordpress.com/2014/01/15/improved-seeding-for-clustering-with-k-means/
http://web.stanford.edu/~hastie/Papers/gap.pdf

Networks:
Finding community structure: https://github.com/upphiminn/jLouvain
Representing communities with a mini-map: https://bl.ocks.org/emeeks/125db75c9b55ddcbdeb5 
Useful network statistic: https://en.wikipedia.org/wiki/Assortativity 
Text clustering:
word2vec and t-SNE: http://www.ghostweather.com/files/word2vecpride/
tfidf 

Good examples of labelling the output of clustering?
https://interactive.twitter.com/game-of-thrones
 

Here the the links @micahstubbs showed:
(apologies for any duplicates :sweat-smile:)

https://github.com/micahstubbs/LinkedinGraphGephi | micahstubbs/LinkedinGraphGephi
https://en.wikipedia.org/wiki/Community_structure#The_Louvain_method | Community structure - Wikipedia
https://github.com/upphiminn/jLouvain | upphiminn/jLouvain: Louvain community detection for Javascript (http://arxiv.org/abs/0803.0476) (http://en.wikipedia.org/wiki/Community_structure#The_Louvain_method).
http://localhost:8181/example/example.html | jLouvain Example
http://bl.ocks.org/emeeks/125db75c9b55ddcbdeb5 | Modularity Mini-Map - bl.ocks.org
http://bl.ocks.org/micahstubbs/raw/5246b8a643393f0753a11b98129a3237/ | Blocks Graph - Readme Mentions
http://bl.ocks.org/micahstubbs/68c2091b07505e0995f7d341790d8f41 | bl.ocks metadata - bl.ocks.org
http://bl.ocks.org/micahstubbs/b35f2560f4205570b3328d1b40de0c6c | Blocks Graph VI - bl.ocks.org
https://en.wikipedia.org/wiki/Assortativity | Assortativity - Wikipedia
http://www.ghostweather.com/files/word2vecpride/ | Word2Vec Vis of Pride and Prejudice
https://interactive.twitter.com/game-of-thrones/#?episode=60 | How every #GameOfThrones episode has been discussed on Twitter

