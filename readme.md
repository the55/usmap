# I recommend using d3

When this project was made, d3.js was young and unproven and had no good story for doing maps. That has changed so much. These days, if you want to do data with a US map, consider using d3. Perhaps via...

* http://datamaps.github.io/
* https://d3-geomap.github.io/map/choropleth/us-states/
* https://github.com/mbostock/d3/wiki/Geo-Projections



# [Javascript/SVG plottable US Map](http://www.the55.net/_11/sketch/us_map)


Requirements:

* [Raphael](http://raphaeljs.com/)
* [gRaphael](http://g.raphaeljs.com/) - just for the mouseover tags
* [ScaleRaphael](http://www.shapevent.com/scaleraphael/) - the scalability

To get something like [demo page](http://www.the55.net/_11/sketch/us_map) use:

    var yourIntendedMapWidth = 600;
    var container = 'dom-id-of-your-container-div';
   
    var paper = new ScaleRaphael(container, 950, 650);
    var map = paper.USMap();
    paper.scaleAll(yourIntendedMapWidth/map.width);
   
    map.plot(38.646908,-90.205994, "St. Louis, MO");
    map.darkenState('MO', 0.07);


## Credits

* this project is built on: [https://github.com/robflaherty/us-map-raphael](https://github.com/robflaherty/us-map-raphael)
* base SVG is from: [http://commons.wikimedia.org/wiki/File:Blank_US_Map.svg](http://commons.wikimedia.org/wiki/File:Blank_US_Map.svg)
* lower 48 coords math: [http://commons.wikimedia.org/wiki/File:Usa_edcp_relief_location_map.png](http://commons.wikimedia.org/wiki/File:Usa_edcp_relief_location_map.png)
* Alaska/Hawaii coords math: [http://www.delphi3000.com/articles/article_4479.asp](http://www.delphi3000.com/articles/article_4479.asp)
