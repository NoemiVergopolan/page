---

title: "HydroBlocks v0.2: enabling a field-scale two-way coupling between the land surface and river networks in Earth system models"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Nathaniel W. Chaney
- Laura Torres-Rojas
- admin
- Colby K. Fisher

# Author notes (optional)
author_notes:
- ""
- ""

# Paper publication date
date: "2021-10-09T00:00:00Z"
doi: "10.5194/gmd-14-6813-2021"

# Schedule webpage page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Geoscientific Model Development*
publication_short:  

abstract: "Over the past decade, there has been appreciable progress towards modeling the water, energy, and carbon cycles at field scales (10–100 m) over continental to global extents in Earth system models (ESMs). One such approach, named HydroBlocks, accomplishes this task while maintaining computational efficiency via Hydrologic Response Units (HRUs), more commonly known as “tiles” in ESMs. In HydroBlocks, these HRUs are learned via a hierarchical clustering approach from available global high-resolution environmental data. However, until now there has yet to be a river routing approach that is able to leverage HydroBlocks' approach to modeling field-scale heterogeneity; bridging this gap will make it possible to more formally include riparian zone dynamics, irrigation from surface water, and interactive floodplains in the model. This paper introduces a novel dynamic river routing scheme in HydroBlocks that is intertwined with the modeled field-scale land surface heterogeneity. Each macroscale polygon (a generalization of the concept of macroscale grid cell) is assigned its own fine-scale river network that is derived from very high resolution (∼ 30 m) digital elevation models (DEMs); the inlet–outlet reaches of a domain's macroscale polygons are then linked to assemble a full domain's river network. The river dynamics are solved at the reach-level via the kinematic wave assumption of the Saint-Venant equations. Finally, a two-way coupling between each HRU and its corresponding fine-scale river reaches is established. To implement and test the novel approach, a 1.0° bounding box surrounding the Atmospheric Radiation and Measurement (ARM) Southern Great Plains (SGP) site in northern Oklahoma (United States) is used. The results show:

1) the implementation of the two-way coupling between the land surface and the river network leads to appreciable differences in the simulated spatial heterogeneity of the surface energy balance, 

2) a limited number of HRUs (∼ 300 per 0.25° cell) are required to approximate the fully distributed simulation adequately, and

3) the surface energy balance partitioning is sensitive to the river routing model parameters.


The resulting routing scheme provides an effective and efficient path forward to enable a two-way coupling between the high-resolution river networks and state-of-the-art tiling schemes in ESMs."


# Summary. An optional shortened abstract.
summary: Although there have been significant advances in river routing and sub-grid heterogeneity (i.e., tiling) schemes in Earth system models over the past decades, there has yet to be a concerted effort to couple these two concepts. This paper aims to bridge this gap through the development of a two-way coupling between tiling schemes and river networks in the HydroBlocks land surface model. The scheme is implemented and tested over a 1 arc degree domain in Oklahoma, United States.


tags: [HydroBlocks, Land Surface Modeling, River Routing]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: https://gmd.copernicus.org/articles/14/6813/2021/gmd-14-6813-2021.pdf
url_code: https://zenodo.org/record/4071692#.Ycyjib1ue3I
url_dataset: ''
url_poster: ''
url_project: https://waterai.earth/hydroblocks/
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: 
#- example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: #example
---

