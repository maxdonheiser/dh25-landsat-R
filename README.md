# Exploring extreme heat: Satellite imagery and spatial analysis with Landsat and R

This guide is a somewhat extended version of a Dataharvest 2025 presentation on how to work with satellite imagery and raster data in R. In particular, it will walk you through navigating and downloading *free* satellite imagery from the [USGS EarthExplorer](https://earthexplorer.usgs.gov/) portal, as well as how to combine that with vector data in R to investigate which neighborhoods in Hamburg are most effected by heat in the summer.

The suggested order of this guide is to start with the [presentation](1_presentation.pdf), which gives a quick overview of the different ways to measure heat and how satellites can actually capture information like temperature. The [EarthExplorer quick-start guide](2_earthexplorer_quickstart.md) will guide you through finding the right images to download. Then, you can learn how to analyse the images in R by working directly with the [R markdown file](3_landst_lst_demo.Rmd) in RStudio (or other code editor of your choice) or following along [in-browser](3_landsat_lst_demo.md).

While this is just one example, this guide can be extended to many types of geospatial analysis (flood, drought, land classification) or products from other satellite missions (Sentinel or other private providers).

If you spot any errors or want to see more examples, please reach out!

## Data Sources

|File|Source|
|----|------|
|[LC08_L2SP_195023_20240502_20240511_02_T1_ST_B10.TIF](data/LC08_L2SP_195023_20240502_20240511_02_T1_ST_B10.TIF)|Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 \[dataset]. U.S. Geological Survey. [https://doi.org/10.5066/P9OGBGM6](https://doi.org/10.5066/P9OGBGM6).|
|[LC09_L2SP_196023_20240501_20240502_02_T1_ST_B10.TIF](data/LC09_L2SP_196023_20240501_20240502_02_T1_ST_B10.TIF)|Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 \[dataset]. U.S. Geological Survey. [https://doi.org/10.5066/P9OGBGM6](https://doi.org/10.5066/P9OGBGM6).|

## Other resources

- [Landsat Collection 2 Surface Temperature](https://www.epa.gov/heatislands/measuring-heat-islands)
- [Which measurement is more accurate: taking Earthʼs surface temperature from the ground or from space?](https://science.nasa.gov/climate-change/faq/which-measurement-is-more-accurate-taking-earths-surface-temperature-from-the-ground-or-from-space/)
- [How we measure temperature and why it matters](https://climate.copernicus.eu/how-we-measure-temperature-and-why-it-matters)
- [Measuring Heat Islands](https://www.epa.gov/heatislands/measuring-heat-islands)
- [Mapping Urban Heat Islands Leads NYC Council Data Team to Landsat](https://www.usgs.gov/news/mapping-urban-heat-islands-leads-nyc-council-data-team-landsat)
- [Landsat Collection 2 Data Dictionary](https://www.usgs.gov/centers/eros/science/landsat-collection-2-data-dictionary)
