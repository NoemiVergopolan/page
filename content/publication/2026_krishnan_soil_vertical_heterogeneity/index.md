---
title: "Soil vertical heterogeneity reduces rootzone soil moisture bias in hyper-resolution land surface model over smallholder agricultural systems"

authors:
- Vishnu U. Krishnan
- admin
- Bhupendra Bahadur Singh
- J. Indu
- Lanka Karthikeyan
date: "2026-09-01T00:00:00Z"
doi: "10.1016/j.agwat.2026.110673"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-09-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Agricultural Water Management*
publication_short: ""

abstract: "Conventional Land Surface Models operating at coarse resolution inadequately represent soil heterogeneity and typically assume soil hydraulic parameters derived from surface-layer texture are uniform across the column. This introduces systematic errors in rootzone soil moisture simulations whenever soil properties vary with depth. This limitation becomes significant for their application over smallholder agricultural systems, where fine-scale heterogeneity strongly influences soil moisture dynamics. We hypothesize that representing soil hydraulic parameters as vertically heterogeneous improves soil moisture by reducing systematic bias. We modified HydroBlocks, a hyper-resolution land surface model, to incorporate vertical heterogeneity over agriculture-dominated basin in India, representing first such applications in India. Both vertically heterogeneous and homogeneous configurations are evaluated against in-situ observations, SMAP L3/L4, ERA5-Land, and GLEAM products. HydroBlocks simulations show strong temporal consistency with macroscale products while capturing higher sub-grid spatial variability, emphasizing their suitability for agricultural landscapes. At in-situ locations, vertical heterogeneity systematically reduces subsurface soil moisture bias by approximately 14% relative to homogeneous configuration, while ubRMSE and correlation remain unchanged, indicating the model's ability to correct the mean state while maintaining temporal consistency. Sobol sensitivity analysis across multiple soil layers and seasons reveals that porosity, Brooks-Corey parameter, and wilting point are most influential, with sensitivities varying across layers and interactions intensifying during the monsoon. These results highlight the seasonal and depth-dependent influence of soil hydraulic parameters on soil moisture. The study also demonstrates the potential of hyper-resolution land surface models with vertical heterogeneity to improve farm-scale simulations and support agricultural water management."

# Summary. An optional shortened abstract.
summary: "Where soil differs with depth, models that carry water-holding properties inferred at the surface down the whole column bias the moisture reaching crop roots. We applied depth-varying properties to a hyper-resolution land surface model resolving individual agricultural fields at 30 meters. Against ground measurements, systematic surface soil moisture biases dropped by about 14%, with error spread and timing unchanged, correcting the mean state rather than daily dynamics."

tags:
- Soil Moisture
- HydroBlocks
- Land Surface Modeling
- Agriculture
- Smallholder Farming
- Parameter Estimation
- Uncertainty Quantification
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: https://doi.org/10.1016/j.agwat.2026.110673
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
  caption: ""
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
