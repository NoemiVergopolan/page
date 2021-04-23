---
title: Crop Yield Prediction 
summary: Combining hyper-resolution land surface modeling and machine learning for predicting crop yields at field scale in Zambia.
tags:
- Soil Moisture
- Agriculture
- Crop Yields
- Hyper-resolution
- Droughts
- HydroBlocks
date: "2021-04-05T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  preview_only: true
  caption: 
  focal_point: Smart

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
slides: example
---


## Combining hyper-resolution land surface modeling and machine learning for predicting crop yields at field scale in Zambia.


We have developed cutting edge methods for predicting crop yields at field scale over large spatial extents based on hyper-resolution hydrological modeling and machine-learning (ML) methods. Our work advances on previous approaches by integrating field-scale hydrological variables into yield prediction, and by more effectively quantifying yield sensitivity to drought. The work has been published recently in the scientific journal HESSD as Vergopolan et al. (2021).

This work focused on maize (corn) yields in Zambia, which is the staple crop of the country and much of sub-Saharan Africa, and therefore a key factor in livelihoods and food security. Our approach has important implications for understanding yield gaps (how low actual yields are compared to what could be achieved with sufficient management and inputs, such as fertiliser).

Figure 1.&nbsp; Mean April values (2000–2018) of soil moisture at 30-m spatial resolution, as simulated by HydroBlocks land surface model. April root zone soil moisture was the most predictive variables in the ML model.
Figure 1. Mean April values (2000–2018) of soil moisture at 30-m spatial resolution, as simulated by HydroBlocks land surface model. April root zone soil moisture was the most predictive variables in the ML model.

The key findings of the work are:

Model skill: The modeling approach was able to estimate maize yields at district scale with comparable or higher skill (R2=0.61, MAE=349 kg ha−1) compared to state-of-the-art approaches based on mechanistic yield models and higher skill than standard empirical approaches based on weather variables or vegetation indices.

Yield estimates: The field-scale results showed a mean maize yield of 1557 kg ha−1 (± 219 kg ha−1) across Zambia, with an overall increasing production trend of 3.5 kg ha−1 y−1 (± 4.6 kg ha−1 y−1) between 2000–2018. The field-scale yields captured maize losses during the 2015/2016 El Niño drought at similar levels to losses reported by the FAO based on actual yield data.

Figure 3.  Annual maize yields (a), coefficient of variation (d), and maize yield trends (g) for the period between 2000–2018 estimated using a random forest model. Each zoom panel (b, c, e, f, h, i) shows the respective estimates at a 250-m resolution for a 50-km x 50-km area.
Figure 3. Annual maize yields (a), coefficient of variation (d), and maize yield trends (g) for the period between 2000–2018 estimated using a random forest model. Each zoom panel (b, c, e, f, h, i) shows the respective estimates at a 250-m resolution for a 50-km x 50-km area.

Drivers of yield: We identified soil moisture as the main driver of maize yield variability at both the district-scale and field-scale. At the district-scale, soil moisture was followed in importance by soil temperature, shrubland percent coverage, and precipitation climatology. Time-varying meteorological predictors (precipitation and air temperature) played a minor role. NDVI-based predictors only showed meaningful contribution when soil moisture and soil temperature predictors were absent.

Figure 2.  The most important predictors for maize yield at the district-scale. The predictors were selected and ranked via Recursive Feature&nbsp;Elimination, with the importance rank shown in terms of delta R . Results are shown for case 1 (considering all the variables), case 2 (without precipitation and air temperature predictors), and case 3 (without soil moisture and soil temperature predictors). Each color represents different categories of predictors data.
Figure 2. The most important predictors for maize yield at the district-scale. The predictors were selected and ranked via Recursive Feature Elimination, with the importance rank shown in terms of delta R . Results are shown for case 1 (considering all the variables), case 2 (without precipitation and air temperature predictors), and case 3 (without soil moisture and soil temperature predictors). Each color represents different categories of predictors data.

Drought impacts: There is a highly non-linear relationship between drought indices and yield losses. However, consistent maize losses are observed when soil moisture or precipitation drop below the 25th percentile. At extreme dry conditions (5th percentile), soil moisture identifies 26% more losses with 21% less uncertainty than precipitation, providing an effective measure of drought impact. Significant yield losses are also predicted when soil temperature exceeded 37.5 ◦C in the early growing season. Drought impacted yields differently across the landscape, with most of the spatial variability coming from soil moisture.

Reference: Vergopolan, N., Xiong, S., Estes, L., Wanders, N., Chaney, N. W., Wood, E. F., Konar, M., Caylor, K., Beck, H. E., Gatti, N., Evans, T., and Sheffield, J.: Field-scale soil moisture bridges the spatial-scale gap between drought monitoring and agricultural yields, Hydrol. Earth Syst. Sci., 25, 1827–1847, https://doi.org/10.5194/hess-25-1827-2021, 2021.


