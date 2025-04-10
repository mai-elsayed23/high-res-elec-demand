The original sub-national total GDP geospatial raster has the same resolution as the base sub-national population count one. Thus, no re-sampling was needed here. However, the total GDP raster was aligned to the population count one to ensure compatibility and consistency when performing further analysis.

**N.B.** In case you use different sources for the input datasets, make sure all the base datasets have the same resolution and are aligned before proceeding further.  The base datasets are: population count, total GDP, and nighttime lights. The developed tool includes functions for raster re-sampling and alignment.

#### Details of output datasets
|Dataset|Type|Spatial extent|Spatial resolution|Temporal resolution|Selected year|Unit|Filename(s) in this folder|
|-------|----|-------------|------------------|-------------------|-------------|----|-----------------------|
|Aligned sub-national total GDP (PPP)|Geospatial raster|Namibia|30 arcsec|Annual for 1990, 2000 & 2015|2015|Constant 2011 international USD|nam_GDP_PPP_2015_1km_aligned.tif|
