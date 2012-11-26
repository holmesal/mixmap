mixmap
======

Pull location+quantity data from mixpanel and display on a map

Getting Started
======

Add your mixpanel key and secret around line 18 in mixmap.py

If you're using google app engine, just change the handlers in the bottom of mix map.py

If you're not using google app engine, you can still use mixmap. Just replace the "features" array around line 49 of templates/mixmap.html with your own data, and you're good to go.

The "f" variable is standard, and is part of the GeoJSON spec (http://www.geojson.org/). Set f.properties.scale to a number between 0 and 1 for each feature (see line 68). This, along with draw_min_size and draw_max_size, determines the size of each marker. Lines 71-72 should take care of all the funky sizing/positioning of the svg.

Enjoy!