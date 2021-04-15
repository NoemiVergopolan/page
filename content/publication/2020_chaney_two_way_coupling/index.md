---

title: "Two-way coupling between the sub-grid land surface and river networks in Earth system models"

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
date: "2020-10-28T00:00:00Z"
doi: "10.5194/gmd-2020-291"

# Schedule webpage page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In *Geoscientific Model Development*
publication_short:  

abstract: "Over the past decade, there has been appreciable progress towards modeling the water, energy, and carbon cycles at field-scales (10–100 m) over continental to global extents. One such approach, named HydroBlocks, accomplishes this task while maintaining computational efficiency via sub-grid tiles, or Hydrologic Response Units (HRUs), learned via a hierarchical clustering approach from available global high-resolution environmental data. However, until now, there has yet to be a macroscale river routing approach that is able to leverage HydroBlocks' approach to sub-grid heterogeneity, thus limiting the added value of field-scale land surface modeling in Earth System Models (e.g., riparian zone dynamics, irrigation from surface water, and interactive floodplains). This paper introduces a novel dynamic river routing scheme in HydroBlocks that is intertwined with the modeled field-scale land surface heterogeneity. The primary features of the routing scheme include: 1) the fine-scale river network of each macroscale grid cell's is derived from very high resolution ($<$ 100 m) DEMs; 2) the inlet/outlet reaches of each macroscale grid cell are linked to assemble the continental river networks; 3) the river dynamics are solved at a reach-level via the Kinematic wave assumption of the Saint-Venant equations; 4) a two-way coupling is established between each sub-grid tile and the river network. To implement and test the novel approach, a 1.0-degree bounding box surrounding the Atmospheric Radiation and Measurement (ARM) Southern Great Plains (SGP) site in Northern Oklahoma (United States) is used. The results show: 1) the implementation of the two-way coupling between the land surface and the river network leads to appreciable differences in the simulated spatial heterogeneity of the surface energy balance; 2) a limited number of tiles (~300 per 0.25-degree cell) are required to approximate the fully distributed simulation adequately; 3) the surface energy balance partitioning is sensitive to the river routing model parameters. The resulting routing scheme provides an effective and efficient path forward to enable a two-way coupling between the high-resolution river networks and existing tiling schemes within Earth system models."


# Summary. An optional shortened abstract.
summary: Drought monitoring and yield prediction often rely on coarse-scale hydroclimate data or (infrequent) vegetation indexes that do not always indicate the conditions farmers face in the field. Consequently, decision-making based on these indices can often be disconnected from the farmer reality. Our study focuses on smallholder farming systems in data-sparse developing countries, and it shows how field-scale soil moisture can leverage and improve crop yield prediction and drought impact assessment. 

tags: [ HydroBlocks, Land Surface Modeling, Machine Learning, River Routing]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: https://gmd.copernicus.org/preprints/gmd-2020-291/gmd-2020-291.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
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
slides: #example

---

