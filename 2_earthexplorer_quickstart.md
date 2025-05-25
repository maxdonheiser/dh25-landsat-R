# EarthExplorer Quick Start Guide

1. Landsat data can be accessed via the EarthExplorer tool: [https://earthexplorer.usgs.gov/](https://earthexplorer.usgs.gov/)
    1. Anyone can access the tool, but some features are only available with a login
    2. Everything is free, including the account
    3. Pay attention to citation guidelines
2. Choose a geographic region of interest
    1. Map doesn't show location names*, so you have to manually find the location (*unless you change the base layer and are looking in the US)
    2. You can use the Geocoder to lookup a location by name or you can manually add coordinates to the map.
    3. Once you found your region of interest, draw a shape around it. This doesn't need to be very detailed.
    4. Alternatively: You can upload the vector data for a region of interest in one of the specified file formats (KML/Shapefile). You must be logged in to do this. Important to note: Super detailed geometries are not necessary for this. A bounding box would suffice.
3. Choose a date range
    1. You can specify a range (i.e. May - August 2024) or choose months across years.
4. Dealing with clouds
    1. Satellites can only accurately capture LST if there are no clouds. If there are clouds, then the measurements will reflect the temperature of the clouds rather than the ground below them
    2. That being said, the built-in cloud coverage filter checks an entire image, not the area of interest
    3. I like to filter my search results to maximum 20 to 50% cloud coverage and then manually inspect whether I can use the images
5. Choose your dataset
    1. Landsat -> Landsat Collection 2 Level 2 -> Landsat 8-9
    2. Note: There's a ton of other data here that you can use for other types of analysis!
6. Browse the results
    1. Check the footprint: This shows the extent of the satellite image. Sometimes, only part of the geometry is captured.
    2. Preview the image to check cloud coverage in your region of interest
    3. Additional research: Sometimes, you may only want images from days where the temperature reached a minimum value. For instance, we only analysed imagery from "summer days", which are classified by the German National Weather Service as reaching a minimum of 25C.
    4. For bulk download, add the images to your cart. If you only need one or two images, you can download directly.
7. Bulk downloading images
    1. You can choose to download all the associated data or just certain files. In this case, we just need to download the data for surface temperature (ST)
    2. Only works in chrome and microsoft edge
