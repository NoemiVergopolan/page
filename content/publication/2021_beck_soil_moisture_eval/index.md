---

title: "Evaluation of 18 satellite- and model-based soil moisture products using in situ measurements from 826 sensors"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Hylke E. Beck
- Ming Pan
- Diego G. Miralles
- Rolf H. Reichle
- Wouter A. Dorigo
- Sebastian Hahn
- Justin Sheffield
- Lanka Karthikeyan
- Gianpaolo Balsamo
- Robert M. Parinussa
- Albert I. J. M. van Dijk
- Jinyang Du
- John S. Kimball
- admin
- Eric F. Wood

# Author notes (optional)
author_notes:
- ""
- ""

# Paper publication date
date: "2021-01-04T00:00:00Z"
doi: "10.5194/hess-25-17-2021"

# Schedule webpage page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Hydrology and Earth System Sciences*
publication_short:  

abstract: "Information about the spatiotemporal variability of soil moisture is critical for many purposes, including monitoring of hydrologic extremes, irrigation scheduling, and prediction of agricultural yields. We evaluated the temporal dynamics of 18 state-of-the-art (quasi-)global near-surface soil moisture products, including six based on satellite retrievals, six based on models without satellite data assimilation (referred to hereafter as “open-loop” models), and six based on models that assimilate satellite soil moisture or brightness temperature data. Seven of the products are introduced for the first time in this study: one multi-sensor merged satellite product called MeMo (Merged soil Moisture) and six estimates from the HBV (Hydrologiska Byrans Vattenbalansavdelning) model with three precipitation inputs (ERA5, IMERG, and MSWEP) with and without assimilation of SMAPL3E satellite retrievals, respectively. As reference, we used in situ soil moisture measurements between 2015 and 2019 at 5 cm depth from 826 sensors, located primarily in the USA and Europe. The 3-hourly Pearson correlation (R) was chosen as the primary performance metric. We found that application of the Soil Wetness Index (SWI) smoothing filter resulted in improved performance for all satellite products. The best-to-worst performance ranking of the four single-sensor satellite products was SMAPL3E$\\_{SWI}$, SMOS$\\_{SWI}$, AMSR2$\\_{SWI}$ and ASCAT$\\_{SWI}$, with the L-band-based SMAPL3E$\\_{SWI}$ (median R of 0.72) outperforming the others at 50 % of the sites. Among the two multi-sensor satellite products (MeMo and ESA-CCI$\\_{SWI}$), MeMo performed better on average (median R of 0.72 versus 0.67), probably due to the inclusion of SMAPL3E$\\_{SWI}$. The best-to-worst performance ranking of the six open-loop models was HBV-MSWEP, HBV-ERA5, ERA5-Land, HBV-IMERG, VIC-PGF, and GLDAS-Noah. This ranking largely reflects the quality of the precipitation forcing. HBV-MSWEP (median R of 0.78) performed best not just among the open-loop models but among all products. The calibration of HBV improved the median R by +0.12 on average compared to random parameters, highlighting the importance of model calibration. The best-to-worst performance ranking of the six models with satellite data assimilation was HBV-MSWEP+SMAPL3E, HBV-ERA5+SMAPL3E, GLEAM, SMAPL4, HBV-IMERG+SMAPL3E, and ERA5. The assimilation of SMAPL3E retrievals into HBV-IMERG improved the median R by +0.06, suggesting that data assimilation yields significant benefits at the global scale. "


# Summary. An optional shortened abstract.
summary: We evaluated the largest and most diverse set of surface soil moisture products ever evaluated in a single study. We found pronounced differences in performance among individual products and product groups. Our results provide guidance to choose the most suitable product for a particular application.

tags: [Soil Moisture, Remote Sensing]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: https://hess.copernicus.org/articles/25/17/2021/hess-25-17-2021.pdf
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

