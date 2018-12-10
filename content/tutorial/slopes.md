+++
title = "Estimating channel slope globally in rivers"

date = 2018-09-09T00:00:00
# lastmod = 2018-09-09T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.

# Add menu entry to sidebar.
linktitle = "Estimating river slope globally"
[menu.tutorial]
  parent = ""
  weight = 3
+++
Estimating the channel slope for the sites in a global database. Currently digital elevation models are largely useful in topographic studies, but its sources are often differnt among countries, and is hard to use globally at a high resolution. Here I did an R script to estimate channel slope from rivers in any part of the globe.
For each site, we downloaded the DEM covering each site hosted in the Amazon Web Services (https://registry.opendata.aws/terrain-tiles/), with a pixel resolution ranging from 9-19 m, depending on the source. For each site within the database (cross) we extracted the elevation of all locations around 500 m of the site (black dots). By finding the location with the lowest elevation (red dot), we assumed that it corresponds to the stream channel downstream. And calculated the slope as the elevation difference divided by the distance. The code can be found in [github](https://github.com/rocher-ros/global_slope/wiki). 

{{< figure library="1" src="slope.png" title="" >}}