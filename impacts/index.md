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

## Drought sensitivity changes of rainfed cereals in Spain assessed with remote sensing

#### with [Sergio Contreras](http://www.futurewater.es/quienes-somos/nuestro-equipo/sergio-contreras-lopez/){:target="_blank"} and [Johannes Hunink](http://www.futurewater.es/quienes-somos/nuestro-equipo/johannes-hunink/){:target="_blank"} ([FutureWater](http://www.futurewater.es/){:target="_blank"}). Submitted to *Journal of Agronomy and Crop Science.*

In the context of global warming, as drought episodes become increasingly frequent, it is crucial to determine whether major cereal crops are becoming more sensitive to drought in order to ensure future national food security. This study uses a 12-year dataset on crop yields and harvested areas for plots throughout Spain to estimate the effects of agricultural droughts on rainfed cereals. To assess drought stress for each location, we used two satellite-based drought indicators: the Vegetation Condition Index (VCI) and the Temperature Condition Index (TCI). We showed that both indicators are good predictors of cereal yields and are able to explain at least 28% of annual yield variation, depending on crop type. Then, we defined a crop-specific **Drought Environment Index** to evaluate changes over time of the sensitivity of yields to drought stress. By looking at each crop, we found that the general stagnation of cereal yields in Spain during the last fifteen years has been accompanied by an increase in resilience of wheat and barley fields to very adverse drought conditions, characterised by very high temperatures and extreme canopy stress. This can possibly be attributed to the development of more drought-resistant seed varieties.

<figure class="half">
	<a href="/images/TR_binary.png"><img src="/images/TR_binary.png"></a>
	<a href="/images/CB_binary.png"><img src="/images/CB_binary.png"></a>
	<a href="/images/AV_binary.png"><img src="/images/AV_binary.png"></a>
	<a href="/images/CN_binary.png"><img src="/images/CN_binary.png"></a>
	<figcaption>Spatial distribution of cereal production in Spain, as derived from the ESYRCE survey. Wheat (upper left), Barley (upper right), Oat (bottom left) and Rye (bottom right).</figcaption>
</figure>

### Main findings

We found that VCI and TCI correlated positively with annual yields, that is, agricultural droughts (characterised by values of these variables below 0.5) generated yield damages that ranged from 2% up to more than 20% depending on the crop and the severity of the drought episode. Moreover, we found that the effect of VCI on yields is intensified as we approach the harvesting phase of crops (Siebert et al. [2017](http://iopscience.iop.org/article/10.1088/1748-9326/aa7f15){:target="_blank"}). On the other hand, TCI had a significant effect on the first and last stages of the growing period (except for rye, in which TCI was relevant in the second and third stages). Despite farm level yields being explained by a large set of local and specific factors, a remarkable amount of yield variability at the field scale was explained only by using these two drought condition indices.

The trend analysis of yields is in agreement with that found by other scientists on the general stagnation of cereal yields in Europe (Ceglar et al. [2016](https://www.sciencedirect.com/science/article/pii/S0168192315007303){:target="_blank"}, [2017](https://www.sciencedirect.com/science/article/pii/S0168192317301247){:target="_blank"}). This study also shows that this trend is general for all varieties, except for rye. Lobell and Moore ([2015](http://www.pnas.org/content/112/9/2670){:target="_blank"}) have found evidence that this applies since the beginning of the 90’s, possibly connected to the action of human-induced climate change.

<figure class="half">
	<a href="/images/TR_detrend_cell_avg_vci.png"><img src="/images/TR_detrend_cell_avg_vci.png"></a>
	<a href="/images/CB_detrend_cell_avg_vci.png"><img src="/images/CB_detrend_cell_avg_vci.png"></a>
	<figcaption>Wheat (left) and Barley (right) average crop yield anomalies (t/ha) for quintiles of Drought Environment Index (DEI) anomaly by year (dashed lines) and best-fit linear regression for each quintile (solid lines).</figcaption>
</figure>

<br>

The Drought Environment Index (DEI) demonstrated to be a valuable index for assessing trends of crop sensitivity to droughts. The analysis of yield anomalies over the study period showed a reduction of wheat and barley sensitivity to extreme drought conditions (characterised by DEI quintiles), and certain improvement in the performance of barley yields under moderate drought conditions, possibly describing an improvement in seed’s drought resilience. No changes in sensitivity were identified for oat or rye while a general increase in productivity was detected for the latter for all levels of drought severity.

---

## A non-parametric approach to describe spatio-temporal yield variation and drought impacts at the farm level: An application to the Po river basin 

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