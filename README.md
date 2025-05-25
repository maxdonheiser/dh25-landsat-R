# Exploring extreme heat: Satellite imagery and spatial analysis with Landsat and R

This guide is a somewhat extended version of a Dataharvest 2025 presentation on how to work with satellite imagery and raster data in R. In particular, it will walk you through navigating and downloading *free* satellite imagery from the [USGS EarthExplorer](https://earthexplorer.usgs.gov/) portal, as well as how to combine that with vector data in R to investigate which neighborhoods in Hamburg are most effected by heat in the summer.

The suggested order of this guide is to start with the presentation [presentation](1_presentation.pdf), which gives a quick overview of the different ways to measure heat and how satellites can actually capture information like temperature. The [EarthExplorer Quick Start Guide](2_earthexplorer_quickstart.md) will guide you through finding the right images to download. If you just want to look at the code, you can jump straight to the [R script](3_landst_lst_demo.Rmd).

While this is just one example, this guide can be extended to many types of geospatial analysis (flood, drought, land classification) or products from other satellite missions (Sentinel or other private providers).

If you spot any errors or want to see more examples, please reach out!

## Data Sources

|File|Source|
|----|------|
|[LC08_L2SP_195023_20240502_20240511_02_T1_ST_B10.TIF](data/LC08_L2SP_195023_20240502_20240511_02_T1_ST_B10.TIF)|Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 \[dataset]. U.S. Geological Survey. [https://doi.org/10.5066/P9OGBGM6](https://doi.org/10.5066/P9OGBGM6).|
|[LC09_L2SP_196023_20240501_20240502_02_T1_ST_B10.TIF](data/LC09_L2SP_196023_20240501_20240502_02_T1_ST_B10.TIF)|Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 \[dataset]. U.S. Geological Survey. [https://doi.org/10.5066/P9OGBGM6](https://doi.org/10.5066/P9OGBGM6).|
|[hamburg.geojson](data/hamburg.geojson)|[Landesbetrieb Geoinformation und Vermessung (LGV) Hamburg](https://www.hamburg.de/politik-und-verwaltung/behoerden/behoerde-fuer-stadtentwicklung-und-wohnen/aemter-und-landesbetrieb/landesbetrieb-geoinformation-und-vermessung)|
