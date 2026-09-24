---
title: "Parameter Estimation in Land Surface Models: Challenges and Opportunities With Data Assimilation and Machine Learning"

authors:
- Nina Raoult
- Natalie Douglas
- Natasha MacBean
- Jana Kolassa
- Tristan Quaife
- Andrew G. Roberts
- Rosie Fisher
- Istem Fer
- Cédric Bacour
- Katherine Dagon
- Linnia Hawkins
- Nuno Carvalhais
- Elizabeth Cooper
- Michael C. Dietze
- Pierre Gentine
- Thomas Kaminski
- Daniel Kennedy
- Hannah M. Liddy
- David J. P. Moore
- Philippe Peylin
- Ewan Pinnington
- Benjamin Sanderson
- Marko Scholze
- Christian Seiler
- T. Luke Smallman
- admin
- Toni Viskari
- Mathew Williams
- John Zobitz
date: "2025-10-28T00:00:00Z"
doi: "10.1029/2024MS004733"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-28T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Journal of Advances in Modeling the Earth System*
publication_short: ""

abstract: Accurately predicting terrestrial ecosystem responses to climate change over long-timescales is crucial for addressing global challenges. This relies on mechanistic modeling of ecosystem processes through land surface models (LSMs). Despite their importance, LSMs face significant uncertainties due to poorly constrained parameters, especially in carbon cycle predictions. This paper reviews the progress made in using data assimilation (DA) for LSM parameter optimization, focusing on carbon-water-vegetation interactions, as well as discussing the technical challenges faced by the community. These challenges include identifying sensitive model parameters and their prior distributions, characterizing errors due to observation biases and model-data inconsistencies, developing observation operators to interface between the model and the observations, tackling spatial and temporal heterogeneity as well as dealing with large and multiple data sets, and including the spin-up and historical period in the assimilation window. We outline how machine learning (ML) can help address these issues, proposing different avenues for future work that integrate ML and DA to reduce uncertainties in LSMs. We conclude by highlighting future priorities, including the need for international collaborations, to fully leverage the wealth of available Earth observation data sets, harness ML advances, and enhance the predictive capabilities of LSMs.

# Summary. An optional shortened abstract.
summary: "Land surface models, which simulate vegetation, soil, water and carbon within Earth system models, depend on parameters that often cannot be measured directly. Varying one carbon flux parameter within its uncertainty range can shift projected atmospheric CO2 in 2100 more than the choice of emissions scenario. This review presents two decades of work on adjusting parameters to match observations is consolidated into seven recurring obstacles, each paired with a machine learning opportunity."
tags:
- Land Surface Modeling
- Parameter Estimation
- Data Assimilation
- Uncertainty Quantification
- Machine Learning
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: https://doi.org/10.1029/2024MS004733
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
  caption: "Schematic of the parameter data assimilation (PDA) workflow for land surface models, illustrating the interactions between model, observations, and assimilation components. Methods ,challenges and future priorities are highlighted."
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

