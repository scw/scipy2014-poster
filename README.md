Modeling The Global Shipping Trade Using A Python-based Analysis Stack
======================================================================

 - [Open the poster](https://github.com/scw/scipy2014-poster/poster-scipy-2014.pdf) (2.5MB PDF)
 - [Download the source](https://github.com/scw/scipy2014-poster/poster-scipy-2014.svg) (5.2MB Inkscape SVG)


Description
-----------

Performing modern-day scientific analysis often requires using tools from multiple domains. Here, a scientific workflow for analyzing the global shipping trade is developed using Python tools for probabilistic record linkage, fuzzy string matching, web scraping, document parsing, geodesic calculations, and raster processing to answer questions about ship movement. 


Abstract
--------

Shipping accounts for 90% of global trade volume, and plays far-reaching economic and ecological roles. Despite this importance, little data is publicly available. This work uses requests, BeautifulSoup and lxml to download and parse billions of ship-based observations collected over radio frequencies using the Automatic Identification System (AIS), initially stored in KML files. These raw observations were filtered into a PostGIS database, which provides geographic primitives and spatial indexing. The data was then validated using probabilistic record linkage and fuzzy string matching using jellyfish to correlate between data sources. Finally, the data was geographically filtered by applying methods from geographiclib, geopy and GDAL in a parallel environment to create a validated model of global ship movement.

A few specific ecological use cases of this data will be discussed, built using spatial Python tools, such as modeling the effect of ship strikes, or ship-whale collisions, based on computed vessel types and velocities, and examining noise pollution from vessel traffic. As streaming data platforms come online, vessel movement can be analyzed in real-time within a geospatial analysis workflow, opening the possibility for dynamic management of ocean resources, which requires integration between scientific computing and heterogenous systems that map well onto Python's existing ecosystem, some implications of which will be discussed.

Bibliography
------------

See the [full thesis](https://github.com/scw/thesis) for a detailed bibliography.
