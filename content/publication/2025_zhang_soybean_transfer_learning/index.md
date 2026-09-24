---
title: "Transfer learning for improved crop yield predictions in a cross-scale pathway: a case study for Brazilian national soybean"

authors:
- Jiaying Zhang
- Kaiyu Guan
- Zhangliang Chen
- Yizhi Huang
- Kejie Zhao
- Bin Peng
- Sheng Wang
- Xiaocui Wu
- Sibo Wang
- Arindam Banerjee
- admin
- Rong Fu
- Siyu Zhao
- Joana Colussi
date: "2025-12-01T00:00:00Z"
doi: "10.1016/j.jag.2025.104981"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-12-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *International Journal of Applied Earth Observation and Geoinformation*
publication_short: ""

abstract: "Crop yield prediction at a fine spatial scale is crucial for improving agricultural management and resource allocations. Many countries and regions lack fine-scale yield data for fine-scale modeling and thus have to use a “cross-scale pathway”, where coarse-scale (e.g., state-level) data are used to train a model for fine-scale (e.g., county-level or field-level) yield predictions. However, the cross-scale pathway has limited effectiveness in predicting yield due to issues with data availability and model scalability. In this study, we quantify the benefits of transfer learning in the cross-scale pathway. We applied transfer learning by fine-tuning a previously trained and validated AI-based machine learning model, originally developed for field-level soybean yield predictions in the United States, using Brazilian state-level data to predict Brazilian municipal-level soybean yield. Despite differences in environmental conditions, crop phenology, and yield responses between the U.S. and Brazil, we show that transfer learning improves the municipal-level predictions from the cross-scale pathway by increasing the R2 from 0.29 (without transfer learning) to 0.44. Notably, this is achieved without using any municipal-level data and relying only on scarce state-level observations. When the municipal-level data were used, the transfer learning achieved an R2 of 0.57, the most stable high performance compared with previous studies. The effectiveness of the cross-scale pathway, thus, increases from 50% to 78% with transfer learning. These findings demonstrate the benefits of transfer learning in the cross-scale pathway under data-limited conditions, and underscore the potential for global crop yield predictions across scales."

# Summary. An optional shortened abstract.
summary: "Many countries report crop yields only for large administrative units, so models trained on coarse records must be applied at finer scales, where few samples and scale-dependent relationships degrade accuracy. A machine learning model trained on field-level soybean yields in the US Midwest was fine-tuned with Brazilian state-by-year records, a technique called transfer learning, then used to predict municipal yields from 2001 to 2021. Transfer across scales rather than across regions had rarely been tested. Without any municipal training data, explained yield variance rose from 0.29 to 0.44, though transfer added little where fine-scale data were plentiful."
tags:
- Agriculture
- Crops
- Yield
- Machine Learning
- Remote Sensing
- Soybean
- Brazil
- Transfer Learning
featured: false

links:
#- name: Custom Link
#  url: 
url_pdf: https://doi.org/10.1016/j.jag.2025.104981
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
