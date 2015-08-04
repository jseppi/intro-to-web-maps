% Basics of Online Maps
% James Seppi
% August 4, 2015

-------------------------------------------------

# Basics of Online Maps

Presentation by James Seppi

Software Developer at [TNRIS](http://tnris.org), part of [TWDB](http://www.twdb.texas.gov)

Twitter: [hydrologee](http://twitter.com/hydrologee)

Viewable at [jseppi.github.io/intro-to-web-maps/](http://jseppi.github.io/intro-to-web-maps/)

Source code at [github.com/jseppi/intro-to-web-maps/](https://github.com/jseppi/intro-to-web-maps/)

# What is an Online Map?

# What is an <s>Online</s> Map?

<h1>What is a Web Map?</h1>

# What is a Web Map?

A cartographic map on a web page

. . .

Can move around (pan) and zoom in and out

. . .

Like [Google Maps](https://www.google.maps/com)

![](img/google-maps.png)

. . .

And also maps from [Bing](https://www.bing.com/maps/), [MapQuest](http://mapquest.com), [ESRI](http://www.arcgis.com/home/webmap/viewer.html?useExisting=1), [Mapbox](http://mapbox.com), [Stamen](http://maps.stamen.com/#terrain/12/37.7706/-122.3782), [CartoDB](https://cartodb.com/), etc. 

# What is a Web Map?

Typically streets or satellite imagery

![[Bing Satellite](http://bing.com/maps)](img/bing-satellite.png)

# What is a Web Map?

Sometimes with a simplified basemap and additional data overlaid

![[apps.texastribune.org/reservoirs/](http://apps.texastribune.org/reservoirs/)](img/tt-reservoirlevels.png)

# What is a Web Map?

Found everywhere these days:

. . .

News sites, food review sites, travel booking sites, data explorers, etc.

----------------------------

<div class="big-image"><img src="img/yelp.png" /></div>

----------------------------

<div class="big-image"><img src="img/airbnb.png" /></div>

----------------------------

<div class="big-image"><img src="img/eater.png" /></div>

----------------------------

<div class="big-image"><img src="img/iswp.png" /></div>

# Why do we care?

Maps are a valuable tool for communication

. . .

Power in communication

. . .

Maps show borders, areas of conquest, impacts of policies, natural phenomenon, etc.

------------------------------

<div class="big-image"><img src="img/borders.png" /></div>

<div class="attr"><a href="http://opennews.kzhu.io/map-disputes/">Source</a></div>

# Why do we care?

By understanding maps and cartography, we have the power to see biases and think critically

. . .

![How to Lie with Maps by Mark Monmonier](img/how-to-lie-with-maps.png)

# Some History

**MapQuest** in 1996

. . .

![](img/mapquest_1996.jpg)

. . .

Driving directions, on the Internet, printable

. . .

<span class="larger">WHOA!</span>

<div class="attr">Mapquest 1996: <a href="http://www.computerhistory.org/revolution/the-web/20/392/2345">Source</a></div>

----------------------

# But it was a little slow

(though so was everything online back then)

. . .

![](img/turtle.jpg)

. . .

Required a full page refresh to pan or zoom

<div class="attr">Tiny Turtle: <a href="https://creativecommons.org/licenses/by-nc-nd/2.0/">CC BY-NC-ND</a>, <a href="https://www.flickr.com/photos/angelskiss31/2472924279/in/photolist-4Lwoev-4TtUqF-ej1p5c-9QVYJB-8B26At-9HKwZ3-rFtkZG-eaLgPs-GhBE4-6vYZp7-71C2A1-9xgbxG-9XPdm-6bqCZa-7Nvxw1-7NryV6-7NvxuG-7NvxrW-8MafHa-6ToUFF-3YKG8-LNtRp-LB2z2-7GJ8B-6niyEU-bug2ir-bie9k2-8nKry-61aWfe-4Q4vnQ-6tDL2L-bTSsNK-7TBreS-49WKWA-54sPet-dFMMHy-aFhfhD-4gRfAc-aFhffM-5L6RAA-5JKQdj-PM62L-5JKQ7o-5JKQad-37qLkZ-efBnyK-83oh7Z-f4ZvM6-oj3orM-7gAnPv">Source</a></div>

# Some History

9 years later, in early 2005

. . .

<span class="larger">Google Maps!</span>

. . .

![](img/old_google_maps.jpg)

. . .

Fluid, continuous panning and zooming

---------------------

<div class="big-image"><img src="img/tim-and-eric-mind-blown.gif" /></div>

# Tile Technology

. . .

![](img/alhambra-tiles.jpg)

<div class="attr">Alhambra Tiles 7: <a href="https://creativecommons.org/licenses/by/2.0/">CC BY</a>, <a href="https://www.flickr.com/photos/robven/3142024214/in/photolist-5MDGkh-95VRZ-ouVA1-66KGDn-qaotmE-onLhdx-6SX2m6-o9KdDb-nSSTGi-pWcepA-aHtBsF-63q5Xt-h2uRRu-bCQDqi-q9CxTN-qcJQVD-5ZCkiG-hqa5CH-En8XK-qdFEjA-4P8bvg-63YJGV-pVFte6-qdoGfB-hgGiZJ-meVoK-pV85k6-69HBqj-PR9cQ-5MDGa3-4PeYHz-8Pgm3g-9vumGC-6RsTYt-4zGa4t-3tpASM-6kbcGU-hqb8fT-qaVW8N-5MzsxP-bkkE5P-q4G6Lm-pMvun-6Y3sM9-38aYez-4gu2oJ-6de9B-3Cmxni-5Mzs8p-afCky">Source</a></div>

# Tile Technology

![](img/ner-tiles.jpg)

<div class="attr">NER Tile Map segment Beverley: <a href="https://creativecommons.org/licenses/by-nc-nd/2.0/">CC BY-NC-ND</a>, <a href="https://www.flickr.com/photos/johngreyturner/394625304/in/photolist-ASymy-ASyJo-ASyDz-ASyvX-bQtmfa-oXsQHL-eYgmQJ-btgqpB-9MK1RC-nDZjmy-7eTCVD-9uPfUD-9sCzr9-tdZEa5-te84EX-tteNmQ-syKbNR-tvhyFb-syKd46-te84op-tdZD7d-syyBm1-tdYrT1-tdYtGw-nE1iek-nWtvja-9L7DUS-9uBpnm-nWopSs-nYg6x2-nDZztu-nDZywu-9wb1AR-au9Dmy-9uyoRM-nWorCb-nYfYKV-9E55Ms-syKcBp-nWbnNt-tdYuC9-ttePZQ-tvhx3S-nDZPZU-nYg6TT-nWox6A-nDZJ1E-nDZgKd-ac8kwZ-2gEMXi">Source</a></div>

# Tile Technology

Tiles are 256 x 256 pixel images

. . .

When positioned next to each other, they look like one big image

---------------

<div class="big-image"><img src="img/tiles-loading.gif" /></div>

# Tile Technology

Tiles are rendered at different **zoom levels** to show different levels of detail

. . .

More detail -> More tiles

. . . 

The number of tiles increases exponentially at each zoom level

. . .

Typically the zoom levels are 0 through 19

# Tile Technology

Zoom level 0: The entire planet in a single tile

. . .

Zoom level 1: The entire planet in 4 tiles

. . .

Zoom level 2: 16 tiles

...

Zoom level 13: 67,108,864 tiles 

...

Zoom level 19: 4^19 tiles

# Tile Technology

![Zoom level 0](img/osm_0_0_0.png)

# Tile Technology

![Zoom level 1](img/osm_level1.png)

# Tile Technology

![Zoom level 13, Row 1871, Column 3372](img/osm_13_1871_3372.png)

# Web Maps in the Future

. . .

<span class="larger">Vector Tiles</span>

. . .

Instead of pre-rendered images, the actual vector shapes (of roads, areas, points, etc.) are sent to your browser

. . .

Map is drawn **on-the-fly** from the vector data and styling information

. . .

Greater interactivity, smoother zooming, better offline capabilities

# Web Maps in the Future

Google Maps has already made the switch for many users, other companies (like Mapbox and ESRI) are also rapidly moving toward them

![](img/google-maps.png)

# Making Your Own Web Map

[Google Maps API](https://developers.google.com/maps/?hl=en)

. . .

[Bing Maps API](https://www.microsoft.com/maps/choose-your-bing-maps-API.aspx)

[ESRI JavaScript API](https://developers.arcgis.com/javascript/)

[OpenLayers](http://openlayers.org/)

. . .

[Leaflet](http://leafletjs.com/) (Personal Favorite)

# But those all require programming

----------------------------

<div class="big-image"><img src="img/cowboy-programmer.gif" /></div>

# CartoDB

[CartoDB](http://cartodb.com) is an online service for geospatial data visualizations

. . .

Or as most people call them, "maps"

. . . 

Built on [PostGIS](http://postgis.net) and [PostgreSQL](http://postgresql.org)

# CartoDB

Easily import data from a variety of formats (spreadsheets, shapefiles, KML)

. . .

Visualize the data in a web map with presets or customized options

Perform simple or complex analyses

Free for up 50 MB of (converted) data

# CartoDB

Sign up at [cartodb.com/signup](https://cartodb.com/signup) for today's exercises

# Exercise 1 - Simple Points

[Natural Earth Data - naturalearthdata.com](http://www.naturalearthdata.com/)

This is a great resource for general cartographic data, and it's public domain!

# Exercise 1 - Simple Points

1. Download [Natural Earth Data Populated Places](http://www.naturalearthdata.com/downloads/50m-cultural-vectors/50m-populated-places/) dataset: [goo.gl/JqPle5](http://goo.gl/JqPle5)

1. (TODO: Finish this)

# Exercise 2 - Polygons

(TODO: Polygon, choropleth exercise)

# Exercise 3 - Earthquakes

(TODO: Earthquakes data from CartoDB library)

1. Download [All Earthquakes for the Last 30 Days](http://earthquake.usgs.gov/earthquakes/feed/v1.0/csv.php) from USGS: [goo.gl/hhoAyK](http://goo.gl/hhoAyK)

1. Step 2

# Exercise 3 - Your Own Data Exploration

Places for data

(TODO: Find a few good sources of data)

- Austin GIS Data

- ESRI Open Data http://opendata.arcgis.com/

- CartoDB Data Repository

# Local Geo Groups

Austin Open Source GIS User Group

[meetup.com/atx-osg](http://www.meetup.com/atx-osg)

![](img/maptimeatx.png)

[meetup.com/MaptimeATX](http://www.meetup.com/MaptimeATX)

# Credits

* [Maptime Anatomy of a Web Map](http://maptime.io/anatomy-of-a-web-map/)