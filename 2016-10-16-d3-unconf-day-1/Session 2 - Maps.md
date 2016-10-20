drid3.unconf 2016
Session 2: 1:30pm
Boardroom
Maps
d3 projections (@fil): http://visionscarto.net/ode-aux-projections-de-d3-js
Ian’s post: https://hi.stamen.com/an-ode-to-d3-js-projections-9d6477d6da0b
Satellite debris fields: http://bl.ocks.org/syntagmatic/dd17d7b62fb4fbb56897
Cartograms help to represent populations rather than geographical area
Bertin projection

Projection transitions:
http://bl.ocks.org/mbostock/3711652 

Why use alternative projections? Or when not to use Mercator?
Don’t use Mercator if you care about relative areas of countries, e.g. for a choropleth
For a small area it generally doesn’t matter too much what projection you use, as long as it is “conformal” - except in specific domains (e.g. where it matters that the land is moving all the time)
Mix tape of election cartograms: https://bl.ocks.org/veltman/c7bfb3d4a3817f7ee0bf2dd19ff058c1 plus WIRED article about it: https://www.wired.com/2016/10/electoral-maps-look-little-different-heres/ 

Map tiles - difficult to use alternative projections, but easier with vector tiles
http://www.mapbox.com/
http://mapzen.com

License suspensions vs poverty rate:
http://maps.ebclc.org/backontheroad/ 
“Mapbox GL is awesome”

How to visualize two different variables on the same map? - license example above is side-by-side

http://cr.littleearth.ca/
Google Maps images plus two different vector tiles, including roads generated on the fly from GeoJSON

Bivariate choropleth:
http://www.joshuastevens.net/cartography/make-a-bivariate-choropleth-map/
(Tufte would say this kind of thing is too hard to decode)
Election results by hue and population density by saturation:
http://www.citylab.com/politics/2012/11/political-map-weve-been-waiting/3908/ 

Turf: can merge overlapping polygons
https://www.mapbox.com/help/intro-to-turf/
http://turfjs.org/examples/turf-merge/ 

Transit App medium post about how their algorithms work:
https://medium.com/transit-app/how-we-built-the-worlds-prettiest-auto-generated-transit-maps-12d0c6fa502f

