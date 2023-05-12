---
title: "A comprehensive assessment of in situ and remote sensing soil moisture data assimilation in the APSIM model for improving agricultural forecasting across the U.S. Midwest"

authors:
- Marissa Kivi
- admin
- Hamze Dokoohaki
date: "2022-10-25T00:00:00Z"
doi: "doi.org/10.5194/hess-27-1173-2023"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-25T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Hydrology and Earth System Sciences*
publication_short: "HESS"

abstract: Today, the most popular approaches in agricultural forecasting leverage process-based crop models, crop monitoring data, and/or remote sensing imagery. Individually, each of these tools has its own unique advantages but is, nonetheless, limited in prediction accuracy, precision, or both. In this study we integrate in situ and remote sensing (RS) soil moisture observations with APSIM model through sequential data assimilation to evaluate the improvement in model predictions of downstream state variables across 5 experimental sites in the U.S Midwest. Four RS data products and in-situ observations spanning 19 site-years were used through two data assimilation approaches namely Ensemble Kalman Filter (EnKF) and Generalized Ensemble Filter (GEF) to constrain model states at observed time steps and estimate joint background and observation error matrices. Then, the assimilation’s impact on estimates of soil moisture, yield, NDVI, tile drainage, and nitrate leaching was assessed across all site-years. When assimilating in situ observations, the accuracy of soil moisture forecasts in the assimilation layers was improved by reducing RMSE by an average of 17% for 10 cm and ~28% for 20 cm depth soil layer across all site-years. These changes also led to improved simulation of soil moisture in deeper soil layers by an average of 12%. Although crop yield was improved by an average of 23%, the greatest improvement in yield accuracy was demonstrated in site-years with higher water stress, where assimilation served to increase available soil water for crop uptake. Alternatively, estimates of annual tile drainage and nitrate leaching were not well constrained across the study sites. Trends in drainage constraint suggest the importance of including additional data constraint such as evapotranspiration. The assimilation of RS soil moisture showed weaker constraint of downstream model state variables when compared to the assimilation of in situ soil moisture. The median reduction in soil moisture RMSE for observed soil layers was lower, on average, by a factor of 5. However, crop yield estimates were still improved overall with a median RMSE reduction of 17.2%. Crop yield prediction was improved when assimilating both in-situ and remote sensing soil moisture observations and there is strong evidence that yield improvement was higher when under water-stressed conditions. Comparisons of system performance across different combinations of remote sensing data products indicated the importance of high temporal resolution and accurate observation uncertainty estimates when assimilating surface soil moisture observations.

# Summary. An optional shortened abstract.
summary: This study provides a framework for direct integration of soil moisture observations collected from soil sensors and satellite imagery into process-based crop models for improving the representation of agricultral systems. The performance of this framework was evaluated across 19 site-years for crop yield, NDVI, soil moisture, tile flow drainage and nitrate leaching.

tags:
- Agriculture
- Soil moisture
- Crops
- Data Assimilation
- SMAP-HydroBlocks
- Nitrate
- Drainage
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: https://hess.copernicus.org/articles/27/1173/2023/hess-27-1173-2023.pdf
url_code: 
url_dataset: 
url_poster: 
url_project: 
url_slides: 
url_source: 
url_video: 

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---

