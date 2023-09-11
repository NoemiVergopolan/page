---
title: "Towards an Optimal Representation of Sub-Grid Heterogeneity in Land Surface Models"

authors:
- Laura Torres-Rojas
- admin
- John D. Herman
- Nathaniel W. Chaney
date: "2022-12-09T00:00:00Z"
doi: "https://doi.org/10.1029/2022WR032233"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-12-09T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Water Resources Research*
publication_short: ""

abstract: One of the persistent challenges of Land Surface Models (LSMs) is to determine a realistic yet efficient sub-grid representation of heterogeneous landscapes. This is particularly important in emulating the fine-scale and nonlinear interactions between water, energy, and biogeochemical fluxes at the land surface. In LSMs, landscape heterogeneity can be represented using sub-grid tiling techniques, which partition macroscale grid cells (e.g., 1°) into smaller units or “tiles.” However, there is currently no formal procedure to define the number of tiles required to adequately represent the heterogeneity of hydrologic processes within a macroscale grid cell, and across spatial scales. To address these challenges, a new approach is presented to diagnose sub-grid process heterogeneity formally and to infer an optimal number of tiles per macroscale grid cell. The approach is demonstrated using the HydroBlocks modeling framework coupled to Noah-MP LSM implemented over a 1.0-degree domain in Western Colorado in the United States. Our results show that (a) a surrogate model can accurately infer the spatial structure of the LSM's time-averaged hydrological fields, with over 95% overall R2 performance in the validation stage; (b) the optimal configurations for a target level of complexity can be determined using a multi-objective Pareto efficiency analysis, which includes the simultaneous representation of the multi-scale heterogeneity of several processes; (c) the use of ∼100 tiles effectively reproduces a quasi-fully distributed LSM setup (i.e., 83,000 tiles) with approximately 1% of the computational expense. This method provides a path forward to efficiently determine the optimal tile configurations for LSMs while simultaneously considering the spatial heterogeneity and spatial accuracy of hydrologic processes.

# Summary. An optional shortened abstract.
summary: In this study we show how a surrogate model can accurately predict the spatial structure of Land Surface Model's (LSM) hydrological output fields. For a target level of complexity, the optimal LSM tile configuration was determined using a multi-objective Pareto efficiency analysis. We found that approximately 100 tiles can effectively reproduce a quasi-fully distributed LSM setup with 1% of the computational cost. This method provides a path forward to efficiently determine the optimal tile configurations for LSMs while simultaneously considering the spatial heterogeneity and spatial accuracy of hydrologic processes.

tags:
- HydroBlocks
- Land Surface Modeling
- Subgrid scheme
- Pareto Optimization
- Machine Learning
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: 2022_TorresRojas_optimal_subgrid.pdf
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

