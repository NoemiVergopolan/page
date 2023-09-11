---
title: Field-scale Crop Yield Prediction 
summary: Satellite observations, physical models, and machine learning combined can enable crop yield prediction at high spatial resolution at data-scarse regions. Learn more about it [here](research/crop_yields_zambia). 

tags:
- Soil Moisture
- Agriculture
- Crops
- Hyper-resolution
- Droughts
- HydroBlocks
date: "2020-10-05T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  preview_only: true
  caption: 
  focal_point: Smart
banner:
  image: 'header.jpg'
  caption: ""
  focal_point: 'center'
#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---


## Combining hyper-resolution land surface modeling and machine learning for predicting crop yields at field scale

The spatial and temporal variability of soil moisture plays an important role in modulating agricultural crop yields. However, limited hydroclimate and yield data hamper drought impact monitoring and assessment at the farm field scale. To bridge this data gap, through my research, I developed an approach for predicting crop yields at field scale over large spatial extents based on hyper-resolution hydrological modeling and machine-learning (ML). This approach advances on previous approaches by integrating field-scale hydrological variables into yield prediction and by more effectively quantifying yield sensitivity to drought. This work has been published recently in the scientific journal HESS ([Vergopolan et al., 2021](https://hess.copernicus.org/articles/25/1827/2021/)). 

This work focused on predicting maize (corn) yields in Zambia, which is the staple crop of the country and much of sub-Saharan Africa, and therefore a key factor in livelihoods and food security. Enabling drought monitoring and crop yield prediction at local-spatial scales has important implications for understanding yield gaps (how low actual yields are compared to what could be achieved with sufficient management and inputs, such as fertilizer).

{{< figure src="Fig1_map_soil_moisture.png" caption="Mean April values (2000–2018) of root zone soil moisture at 30-m spatial resolution, as simulated by HydroBlocks land surface model. April root zone soil moisture was the most predictive variables in the ML model." numbered="true" >}}

The key findings of the work are:

**Model skill**: The modeling approach was able to estimate maize yields at district scale with comparable or higher skill (R$^2$=0.57 and MAE=310 kg/ha using a year-based cross-validation approach) compared to state-of-the-art approaches based on mechanistic yield models and higher skill than standard empirical approaches based on weather variables or vegetation indices.

**Yield estimates**: The field-scale results showed a mean maize yield of 1557 kg/ha (± 219 kg/ha) across Zambia, with an overall increasing production trend of 3.5 kg/ha/yr (± 4.6 kg/ha/yr) between 2000–2018. The field-scale yields captured maize losses during the 2015/2016 El Niño drought at similar levels to losses reported by the FAO based on actual yield data.

{{< figure src="Fig4_map_composite_300.png" caption="Annual maize yields (a), coefficient of variation (d), and maize yield trends (g) for the period between 2000–2018 estimated using a random forest model. Each zoom panel (b, c, e, f, h, i) shows the respective estimates at a 250-m resolution for a 50-km x 50-km area." numbered="true" >}}

**Drivers of yield**: We identified soil moisture as the main driver of maize yield variability at both the district-scale and field-scale. At the district-scale, soil moisture was followed in importance by precipitation climatology, soil temperature, soil water storage, and cropland intensity. Time-varying meteorological predictors (precipitation and air temperature) played a minor role. NDVI-based predictors only showed meaningful contribution when soil moisture and soil temperature predictors were absent.

{{< figure src="Fig3_feature_importance_comparison.png" caption="The most important predictors for maize yield at the district-scale. The predictors were selected and ranked via Recursive Feature Elimination, with the importance rank shown in terms of delta R$^2$. Results are shown for case 1 (considering all the variables), case 2 (without precipitation and air temperature predictors), and case 3 (without soil moisture and soil temperature predictors). Each color represents different categories of predictors data." numbered="true" >}}

**Drought impacts**: There is a highly non-linear relationship between drought indices and yield losses. However, consistent maize losses are observed when soil moisture or precipitation drop below the 25th percentile. At extreme dry conditions (5th percentile), soil moisture identifies 26% more losses with 21% less uncertainty than precipitation, providing an effective measure of drought impact. Significant yield losses are also predicted when soil temperature exceeded 37.5 $^{\circ}$C in the early growing season. Drought impacted yields differently across the landscape, with most of the spatial variability coming from soil moisture.

**Data Availability**: The annual maize yield maps are available for download [here](https://drive.google.com/drive/folders/13SvABThdEAIg-VuiGtI-hCfouLIYB-jb?usp=sharing) in GeoTIFF format, other hydroclimate data generated as part of this study are also available upon request.

### Reference:

Vergopolan, N., Xiong, S., Estes, L., Wanders, N., Chaney, N. W., Wood, E. F., Konar, M., Caylor, K., Beck, H. E., Gatti, N., Evans, T., and Sheffield, J.: Field-scale soil moisture bridges the spatial-scale gap between drought monitoring and agricultural yields, Hydrol. Earth Syst. Sci., 25, 1827–1847, [https://doi.org/10.5194/hess-25-1827-2021](https://doi.org/10.5194/hess-25-1827-2021), 2021.


