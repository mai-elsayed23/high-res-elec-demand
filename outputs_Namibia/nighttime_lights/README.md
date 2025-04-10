The original sub-national nighttime lights geospatial raster has a higher resolution than the base sub-national population count one. Thus, it was downsampled to 30 arcsec first. Furthermore, it was aligned to the population count raster to ensure compatibility and consistency when performing further analysis.

**N.B.** In case you use different sources for the input datasets, make sure all the base datasets have the same resolution and are aligned before proceeding further. The base datasets are: population count, total GDP, and nighttime lights. The developed tool includes functions for raster re-sampling and alignment.

#### Details of output datasets
|Dataset|Type|Spatial extent|Spatial resolution|Temporal resolution|Selected year|Unit|Filename(s) in this folder|
|-------|----|-------------|------------------|-------------------|-------------|----|-----------------------|
|Downsampled sub-national nighttime lights|Geospatial raster|Namibia|30 arcsec|Annual for 2012-2023|2022|VIIRS annual masked average in nW/cm^2/sr|nam_nighttime_lights_2022_30arcsec.tif|
|Aligned sub-national nighttime lights|Geospatial raster|Namibia|30 arcsec|Annual for 2012-2023|2022|VIIRS annual masked average in nW/cm^2/sr|nam_nighttime_lights_2022_aligned.tif|
