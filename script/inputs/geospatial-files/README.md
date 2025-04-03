Generally, the required input files are as follows:
- Vector shapefiles of the study region borders. For a country, this can be at different administrative levels depending on user preferences.
- High-resolution geospatial raster of population count for the base year, i.e. 2015.
- High-resolution geospatial raster of total gross domestic product for the base year, i.e. 2015.
- High-resolution geospatial raster of nighttime lights for a recent year, e.g. 2022.

**N.B.** The coordinate reference system for all geospatial files should be WGS84.

**N.B.B.** The files uploaded here to the **inputs/geospatial-files** folder are for the Namibian illustrative case study. Files for other study regions can be downloaded from the sources listed below. Except for the study region borders, the other files cover the entire globe. The user can then clip them to the desired study region using that region's administrative borders, and then upload them to be used as inputs in the main script.

#### Details of input datasets
|Dataset|Type|Spatial extent|Spatial resolution|Temporal resolution|Selected year|Unit|Source|Filename(s) in this folder|
|-------|----|-------------|------------------|-------------------|-------------|----|------|-----------------------|
|Study region borders|Vector shapefile|Global|Varies; administrative level 0 - level 3|N/A|N/A|N/A|[GADM data version 4.1](https://gadm.org/download_country.html)|nam_admborders_lvl_0.shp, nam_admborders_lvl_1.shp|
|Sub-national population count|Geospatial raster|Global|30 arcsec|5-year intervals for 1975-2030|2015|Population per grid cell|[Global Human Settlement Layer](https://human-settlement.emergency.copernicus.eu/download.php?ds=pop)|NAM_GHS_popcount_2015_30arcsec.tif|
|Sub-national total GDP (PPP)|Geospatial raster|Global|30 arcsec|Annual for 1990, 2000 & 2015|2015|Constant 2011 international USD|Kummu et al. - [paper](https://doi.org/10.1038/sdata.2018.4), [data](https://datadryad.org/dataset/doi:10.5061/dryad.dk1j0)|nam_GDP_PPP_2015_30arcsec.tif|
|Sub-national nighttime lights|Geospatial raster|Global|15 arcsec|Annual for 2012-2023|2022|VIIRS annual masked average in nW/cm^2/sr|Earth Observation Group - [website](https://eogdata.mines.edu/products/vnl/), [data](https://eogdata.mines.edu/nighttime_light/annual/v22/2022/)|nam_nighttime_lights_2022.tif|
