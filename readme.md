# [Javascript/SVG plottable US Map](http://the55.net/_11/sketch/us_map)


Requirements:

* [Raphael](http://raphaeljs.com/)
* [gRaphael](http://g.raphaeljs.com/) - just for the mouseover tags
* [ScaleRaphael](http://www.shapevent.com/scaleraphael/) - the scalability

To get something like [demo page](http://the55.net/_11/sketch/us_map) use:

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
