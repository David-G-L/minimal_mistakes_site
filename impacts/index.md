---
layout: page
title: 
tags: [drought stress, drought environment index, cereal yields, rainfed crops, remote sensing, statistical crop modelling]
comments: true
share: false
image:
  feature: feat_image_dgl03.jpg
---

>The use of **statistical methods** to approach the relationship between yields and meteorological variables has proliferated during the last decade. This is attributable to the increasing availability and improved quality of observed data, the development of computer tools that can handle big data sets, and the adoption of new observation techniques, like **remote sensing**. Schlenker and Roberts ([2009](http://www.pnas.org/content/106/37/15594){:target="_blank"}) is a prominent example of this stream of literature. Some authors, like Lobell ([2010](http://link.springer.com/chapter/10.1007%2F978-90-481-2953-9_5){:target="_blank"}), claim that, under certain circumstances, this approach would beat the explanatory and forecasting performance of traditional crop models.

---

## Hydro-meteorological versus remote sensing drought indicators as explanatory factors of crop yields in water-limited areas: A case study of Spain’s agricultural districts

#### with [Sergio Contreras](http://www.futurewater.es/quienes-somos/nuestro-equipo/sergio-contreras-lopez/){:target="_blank"} and [Johannes Hunink](http://www.futurewater.es/quienes-somos/nuestro-equipo/johannes-hunink/){:target="_blank"} ([FutureWater](http://www.futurewater.es/){:target="_blank"}). Submitted to *Agricultural Water Management.*

In the context of global warming, as drought episodes become increasingly frequent, it is crucial to understand how to efficiently measure agricultural drought impacts on crops. In particular, it is not clear whether statistical crop models based on more traditional and coarser meteorological indicators of droughts perform better than those based on remotely sensed indicators. We empirically assessed this hypothesis using a spatially detailed, 12-year (2003-2015) dataset on crop yields and harvested areas for plots throughout Spain to estimate statistical crop models of major winter cereals.  Yields and composite drought indicators were spatially aggregated at the Comarca Agraria level (agricultural district). We measured agricultural drought stress using the Standardised Precipitation Index (SPI) at different temporal aggregation and two remote sensing Vegetation Indicators (VIs): the Vegetation Condition Index (VCI) and the Temperature Condition Index (TCI), and their combination. 

<figure class="half">
	<a href="/images/TR_binary.png"><img src="/images/TR_binary.png"></a>
	<a href="/images/CB_binary.png"><img src="/images/CB_binary.png"></a>
	<a href="/images/AV_binary.png"><img src="/images/AV_binary.png"></a>
	<a href="/images/CN_binary.png"><img src="/images/CN_binary.png"></a>
	<figcaption>Spatial distribution of cereal production in Spain, as derived from the ESYRCE survey. Wheat (upper left), Barley (upper right), Oat (bottom left) and Rye (bottom right).</figcaption>
	<br>
</figure>


We showed that remote sensing based models were superior to SPI-based for all crops, both for yield levels and yield anomalies. More specifically, VCI/TCI models of winter wheat and barley were able to explain 70% and 40% of yield levels and yield anomalies variability, respectively. We additionally showed that the goodness of fit of remote sensing based models increased as pixels lying on urban areas were removed from the analysis. Finally, we observed gains in explanatory power when models for climatic zones (instead of models at the national scale) were built. All of our results were cross-validated on subsamples of the whole dataset and on individually fitted models to each Comarca Agraria and their predictive accuracy was assessed on a real-time forecasting exercise. The results of this study point the need to feed agricultural tools, such as agricultural drought early warning systems, crop yield forecasting models and water resource management tools with more local, high-resolution remotely sensed drought data in detriment of spatially coarser precipitation grids.

---

## A non-parametric approach to describe spatio-temporal yield variation and drought impacts at the farm level: An application to Puglia and the Po river basin 

#### with Raúl López, Andrea Toreti and Mateo Zampieri ([Joint Research Centre](https://ec.europa.eu/jrc/en/mars){:target="_blank"}). Work in progress.

The purpose of this research project is to advance in describing the role of remote sensing drought indicators as explanatory factors of rainfed crop yields using empirical crop models. From this research phase, an early warning drought classification system could be extracted.

### Data

**Weather and Remote Sensing data**

- Meteorological indicators (temperature, precipitation) from weather stations: Local network of stations in the Po Valley, as the network is dense enough and available. 

- [fAPAR](http://land.copernicus.eu/global/products/fapar){:target="_blank"} from Copernicus. Indicator on crop photosynthetic activity. 

- [Actual evapotranspiration](https://lpdaac.usgs.gov/dataset_discovery/modis/modis_products_table/mod16a2_v006){:target="_blank"} from MODIS. This product provides global ET at 1km spatial resolution in 8-days composites. The estimation of ET is based on the energy balance approach.

- [Superficial soil moisture](http://www.esa-soilmoisture-cci.org/node/145){:target="_blank"} from radar imagery. It is available since 1979 up to present and the SSM is estimated through a combination of passive and active radar sensors. The spatial resolution is 0.25 degrees (approx. 25 km).

- Land Surface Temperature (LST), from thermal imagery. This product is available since 1981.

**Yield data**. [RICA](http://www.rica.inea.it/public/it/index.php){:target="_blank"} dataset on yield and other agricultural variables over the Po Valley.

### Methods 

We will adapt the methodology of García-León et al. ([2017]({{ site.url }}/impacts/)) to this case study. An empirical crop model is estimated using meteorological and biophysical remote sensing observations

$$yield=\alpha+\beta*province+\delta*year+X^{'}\gamma+u$$

Yield anomalies will be defined as

$$Z=yield-\hat{\alpha}+\hat{\beta}*province+\hat{\delta}*year$$

Sensitivity of yields could be explored by looking at the **Drought Environment Index** (DEI)

$$DEI=\hat{yield}-\hat{\alpha}+\hat{\beta}*province+\hat{\delta}*year=X^{'}\hat{\gamma}$$

Following Zampieri et al ([2017](http://iopscience.iop.org/article/10.1088/1748-9326/aa723b/meta)), construct a tailor-made Combined Stress Indicator (CSI) as yield explanatory factor, using non-parametric techniques: LOESS detrending and ridge linear equations.

 
$$CSI=a*METEO_{detrend}+b*RS_{detrend}$$

Given the discontinuity of farms surveillance, it is proposed to work on a longitudinal framework. Working at the strata level (economic dimension of farms) seems also interesting.