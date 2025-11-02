---
title: "From Soil Moisture Spatial Patterns to Catchment Nitrate Dynamics Using Explainable AI"

authors:
- Felipe Saavedra
- admin
- Andreas Musolff
- Ralf Merz
- Zhenyu Wang
- Carolin Winter
- Larisa Tarasova
date: "2025-11-01T00:00:00Z"
doi: "10.1029/2025WR040295"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-11-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Water Resources Research*
publication_short: ""

abstract: Catchment wetness and related hydrological connectivity determine nitrate mobilization, transport and transformation. However, quantifying connectivity at this scale remains challenging. In this study, we tackle this challenge by developing a multi-branch Deep Learning framework trained on streamflow observations and SMAP-Hydroblocks, a unique satellite-based soil moisture data set at 30 m resolution (aggregated here to 1 km) over the US. We hypothesize that spatial patterns of soil moisture are indicative of the relationship between hydrological connectivity and nitrate transport at the catchment scale, and can be a use to predict nitrate concentrations in the streams. We tested this hypothesis using the developed framework to simulate daily nitrate concentration simultaneously at the outlets of eight catchments with varying land cover and concentration-discharge (C-Q) patterns. Our model satisfactorily represents nitrate dynamics in the study catchments with a median 0.62 Nash-Sutcliffe Efficiency. Spatial patterns of soil moisture on average account for 32% of model feature importance and model performance deteriorates on average by 14% if these patterns are not considered. Leveraging explainable AI (XAI) we confirm that model decisions align with known physical processes across catchments with contrasting C-Q behavior. Attention maps identified near-stream hotspots as the regions with the highest predictive power for nitrate export suggesting a potential link between the soil moisture patterns and catchment-scale hydrological connectivity. This proof-of-concept study demonstrates the potential of XAI combined with high-resolution remote sensing products for improving nitrate predictions and mapping critical areas for nitrate export..

# Summary. An optional shortened abstract.
summary: Nitrate pollution in streams is a significant environmental challenge, affecting water quality and ecosystem health. Hydrological connectivity, the way water moves through the landscape, governs nitrate transport and transformation, but measuring it across entire catchments remains a challenge. Spatial patterns of soil moisture can provide key insights into catchment-scale hydrological connectivity, yet they have not been widely integrated into nitrate prediction models. In this study, we developed a deep learning framework trained on daily streamflow data and SMAP-HydroBlocks, a high-resolution satellite-based soil moisture data set. We tested whether deep learning models can predict nitrate concentrations using spatial soil moisture patterns and applied Explainable AI (XAI) methods to identify which areas contribute most to the model predictions. Our findings reveal that soil moisture patterns significantly improve nitrate predictions, with near-stream areas having the highest predictive power. This study highlights the potential of AI-driven approaches to provide spatially detailed insights into nitrate transport, which could support better water quality management and help identify nutrient pollution hotspots at fine spatial scales.


tags:
- Soil moisture
- SMAP-HydroBlocks
- Nitrate
- Deep learning
- Explainable AI
- Hydrological connectivity
- Remote sensing
- Concentration–discharge
- Catchment modeling
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: https://doi.org/10.1029/2025WR040295
url_code: 
url_dataset: 
url_poster: 
url_project: 
url_slides: 
url_source: 
url_video: 

# To use, add an image named `featured.jpg/png` to your page's folder. 
# Featured image
image:
  filename: "featured.jpg" 
  caption: "Attention maps of computed as absolute SHAP values (a) and (d) show median attention maps across the test period; (b) and (e) show the difference between attention maps during periods with high nitrate concentrations; (c) and (f) show the difference between attention maps during the periods associated with high levels of hydrological connectivity."
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

