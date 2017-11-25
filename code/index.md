---
layout: page
title: 
share: false
comments: false
---

###Resources to convert Remote Sensing objects to Time Series

To perform time series and regression analysis, satellite imagery first needs to be transformed into a suitable format. I highlight next four different methods to convert satellite observation (typically in .HDF or .NetCDF format) to .csv, .Rda files.

- **ENVI-IDL**: Proprietary remote-sensing software that provides hyperspectral image analysis, image enhancement and feature extraction. Usually served with IDL, a programming software used for data analysis, visualization and cross-platform application development. [[link](http://www.harrisgeospatial.com/SoftwareTechnology/ENVI.aspx){:target="_blank"}]

- **MODIStsp**: R package devoted to automatizing the creation of time series of raster images derived from MODIS Land Products data. [[link](http://lbusett.github.io/MODIStsp/){:target="_blank"}]

- **Google Earth Engine - javascript console**: A multi-petabyte catalogue of satellite imagery and geospatial datasets with planetary-scale analysis capabilities that makes it available for scientists, researchers, and developers to detect changes, map trends, and quantify differences on the Earth's surface. [[link](https://code.earthengine.google.com/){:target="_blank"}]

- **Google Earth Engine - Command line** (Requires [Google Earth Engine Python API](https://developers.google.com/earth-engine/python_install){:target="_blank"}) [[link](http://www.khufkens.com/2017/07/22/google-earth-engine-time-series-subset-tool/){:target="_blank"}]

<br>

### Other codes

- **vwIRF**: R function to build visually weighted time paths [[link](https://github.com/David-G-L/vwIRF){:target="_blank"}] [[Description of the code]]({{ site.url }}/code/vwIRF_explained.html){:target="_blank"}

- **DGL02_shiny**: Interactive [R-Shiny](http://shiny.rstudio.com/){:target="_blank"} app that displays interactive graphs [[link](https://github.com/David-G-L/DGL02_shiny){:target="_blank"}]
 
- **Thesis template**: Doctoral thesis [LaTeX](https://miktex.org/){:target="_blank"} template files. Thanks to Enrique Moral-Benito (Bank of Spain), who provided original version [[link](https://github.com/David-G-L/Thesis-template){:target="_blank"}]