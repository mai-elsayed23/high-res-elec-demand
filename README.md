# Spatio-temporal projection of electricity demand for previously un-electrified populations
This repository contains the Apache-2.0 licensed source code for a novel method developed to estimate and project the electricity demand of previously un-electrified populations using a high spatiotemporal resolution.
The original conference paper outlines the complete method and all data sources used (link to the paper will be provided here once it is available).

## Getting the source code
There are two recommended options for getting and working with the source code.

If you are a **modeller** who would like to apply this tool to different case study regions, it is recommended to download a local copy of the repository to your device.
Downloading would give you the most recent version of all the files, without historical versions. Any changes you make to the source code will also remain on your local device.

If you are a **developer** who would like to expand the functionalities of this tool, it is recommended to clone the repository. Instructions for cloning can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). It is recommended to use branching to streamline collaboration for expanding and/or improving the current tool.

## Motivation
This tool has been developed and tailored for the energy landscape of developing countries with low electricity access rates. The purpose of this tool is to provide a relatively simple and open-access method to estimate the electricity demand of previously un-electrified populations with high spatial and temporal resolutions. The results can then be used as an input to other energy simulation/optimisation tools to devise medium- to long-term energy transition strategies and/or electrification planning tools to devise cost-optimal electrification strategies. The results are best suited for use with GIS-based energy modelling tools. Intended users include energy specialists, energy researchers, and students.

## Methodology in brief
This tool utilises socio-economic indicators as driving factors for electricity demand development. Some of these indicators are population size, total gross domestic product (GDP), and income level. High-resolution geospatial datasets for these underlying socio-economic indicators are first obtained/developed for the base year. This step is necessary to obtain the distribution of these indicators on a sub-national level.

Development scenarios, e.g. the Shared Socioeconomic Pathways, are used to obtain the development of said indicators over the years under different scenarios. The base year distribution is used in combination with development scenarios to obtain highly resolved projections for these underlying socio-economic drivers.

Satellite imagery for nighttime lights is used to determine the location of currently un-electrified population clusters. The socio-economic indicators corresponding to these clusters are then used to estimate their electricity demand level based on a global correlation between income level and average electricity demand. The population size of each cluster is then used to calculate its total annual electricity demand. Furthermore, the electricity demand of each populated cluster is classified according to the Multi-Tier Framework (MTF) for electricity access. Results are saved in high-resolution geospatial rasters, and summary statistics can be easily calculated.

So far, this tool can be used for residential electricity demand estimation. Other end uses, like commercial and industrial, are planned to be included in future versions of this work.

The user can expect the following outputs:
- High-resolution population count maps for each scenario and year
- High-resolution total GDP maps for each scenario and year
- High-resolution income level maps for each scenario and year
- High-resolution total residential electricity demand maps for each scenario and year
- High-resolution residential electricity demand per capita maps for each scenario and year
- High-resolution MTF classification maps for each scenario and year

The highest spatial resolution that can be obtained is 30 arc seconds, which is equivalent to 1 km at the equator. This is limited by the spatial resolution of the base year datasets of socio-economic indicators. The highest temporal resolution that can be obtained is annual, starting from 2020 up to 2100. Any number of development scenarios can be modelled as long as these scenarios include the quantified development of essential socio-economic indicators, i.e. population size and total GDP, for the study region. The definition of a study region in this tool is versatile, meaning that any region from sub-national scale to global scale can be practically modelled (subject to input data availability).

## Author information
This work has been developed in the Laboratory of Electricity Market and Power Systems at the Lappeenranta-Lahti University of Technology (LUT) in Finland.

Corresponding author: Mai ElSayed, Junior Researcher, [ORCID profile](https://orcid.org/0000-0001-7534-3508)

Corresponding e-mail: mai.elsayed@lut.fi
