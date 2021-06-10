---
reading_time: true
commentable: false
date: "2020-12-31T00:00:00+01:00"
draft: false
author: admin
editable: false
image:
  placement: 1
  caption: ''
  focal_point: 'center'
  preview_only: yes
header:
  image: "HydroBlocks/header.gif"
  caption: ""
  focal_point: 'center'
tags:
- Land Surface Modeling
- Hyper-resolution
- HydroBlocks
share: true
title: ""
summary: 
type: "page"
url: "HydroBlocks/"

# Shortcodes - to add various content to the webpage
# https://gohugo.io/content-management/shortcodes
---
# HydroBlocks
## A field-scale resolving land surface model over continental extents

HydroBlocks is a hyper-resolution field-scale resolving land surface model that accounts for the water, energy, and carbon balance to solve land surface processes at high spatial and temporal resolutions. HydroBlocks leverages the repeating spatial patterns over the landscape by implementing a hierarchical clustering algorithm to define its computational mesh ([Chaney et al., 2016](https://doi.org/10.1002/hyp.10891); [2020](../publication/2020_chaney_two_way_coupling)). This algorithm clusters the fine-scale drivers of the landscape spatial heterogeneity (e.g., 30-m land cover, soil properties, topography data) into complex tiles/clusters of similar hydrologic behavior (i.e., hydrological response units, HRUs). In this way, by simulating hydrological processes with HRUs instead of regular grids, HydroBlocks yields an effective 30-m spatial resolution while leveraging the complex physics of land surface models and reducing the computational requirements (Figure 1).

{{< figure src="scheme.png" caption="HydroBlocks uses a hierarchical clustering scheme to define the hydrologic response units (HRUs) by clustering the high-resolution drivers of the landscape heterogeneity. The top illustration shows a simplistic example with 3 HRUs. In reality, 100--300 HRUs may be needed to represent the landscape heterogeneity of a catchment. In HydroBlocks, the HRUs interact with each other via surface and subsurface flow." numbered="true" width="70%" >}}

The core of HydroBlocks is the Noah-MP vertical land surface scheme ([Niu et al., 2011](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2010JD015139)) applied to the HRU framework to explicitly represent the spatial heterogeneity of surface processes down to field scale. More specifically, at each time step, the land surface scheme updates the hydrological states at each HRU, and the HRUs dynamically interact laterally via surface and subsurface flow (Figure 1). The subsurface lateral flow is solved by computing the Darcy flux between adjacent HRUs at each subsurface level. Subsequently, these fluxes are added as divergence terms to their corresponding subsurface level of the vertical one-dimensional solution of Richards’ equation in Noah-MP. For surface flow, we developed a dynamic river routing scheme that allows a two-way coupling between the river network and the land surface, including the simulation of floodplain inundation dynamics and its interaction with land processes (Figure 2, and more details [here](../publication/2020_chaney_two_way_coupling)).

{{< figure src="scheme_coupling.png" caption="Illustration of the impact of floodplain inundation dynamics on the land surface. We show the annual mean sensible heat flux, latent heat flux, root zone soil moisture, and land surface temperature. The left column shows the results for the uncoupled simulations (i.e., the routing scheme does not interact with the land surface), while the right column shows the coupled simulations. Source: [Chaney et al., 2020](../publication/2020_chaney_two_way_coupling)." numbered="true" width="100%" >}}

#### Model development and code availability
HydroBlocks has been under development in a collaborative effort between Princeton University and the [Chaney Lab](http://www.chaneylab.earth/) at Duke University. The model source code is available at [Github](https://github.com/chaneyn/HydroBlocks).


## Applications for soil moisture monitoring

Through my research, I applied HydroBlocks for simulating soil moisture at field scales across continental extents. The visualization below shows surface soil moisture at a 3-hour 30-meter resolution across the United States. 

![](../../assets/media/HydroBlocks/header.gif)

We can observe that the soil moisture variability is mainly driven by the rainfall events, as the soil wets with the advance of rainfall storms. By interacting with the landscape, soil moisture gets redistributed to the valleys and riparian zones until it eventually dries down. We can also observe the different memories of soil moisture dry downs across the U.S. With fast and punctual wetting events happening in most of the West and slower and widespread wetting fronts in most Central and Northeastern U.S. Insets of this simulation are also ilustrated in Figures 3 and 4. 

{{< figure src="slide2.png" caption="HydroBlocks surface soil moisture simulation over the California Bay Area on January 3rd, 2017. For illustration and comparison a Landsat image is shown on the left." numbered="true" >}}

At the local scales, we can observe the richness of details of the soil moisture data at 30-meter resolution. The spatial variability is observed in the interactions with the landscape. For example, urban areas tend to show the driest soil moisture due to their impervious coverage. On the other hand, the mountains, with their grassland coverage, show slightly wetter conditions. We also can observe the impact of wetlands, lakes, and river reaches, modulating the soil moisture spatial variability in the riparian zone

{{< figure src="simualtions2.png" caption="HydroBlocks surface soil moisture simulation over the Mississippi River on April 1st 2017. " numbered="true" width="100%" >}}

Figure 4 shows an inset of HydroBlocks simulations over the lower Mississippi River floodplain. The model captures well the soil moisture dynamics at the floodplain, the recharge of river reaches and riparian zones, as well as the heterogeneity associated with the meandric sand dunes. On the right, we also observe the impact of reservoirs controlling soil moisture dynamics locally and downstream. In the floodplain, we can also observe the impact of small reservoirs and paddy irrigated rice farms typical of the region.


#### Data fusion with satellite observations

To improve the accuracy of such detailed soil moisture estimates, we developed an approach to combined HydroBlocks with satellite observations from the NASA's Soil Moisture Active-Passive (SMAP) mission using a novel cluster-based spatial Baeysian merging scheme ([Vergopolan et al., 2020](../publication/2020_vergopolan_combining/)). This approach allowed us to develop [SMAP-HydroBlocks](../SMAPHB), the first hyper-resolution satellite-based surface soil moisture dataset over the continental United States. More details [here](../SMAPHB). 

#### Crop yield modeling and prediction

The strong spatiotemporal variability of soil moisture plays an important role in modulating agricultural crop yields. Through my research, I developed an approach for predicting crop yields at field scale and over large spatial extents based on hyper-resolution hydrological modeling and machine learning ([Vergopolan et al., 2021](../publication/2021_vergopolan_yield_mapping/)). This approach advances on previous approaches by integrating HydroBlocks' field-scale hydrological variables into yield prediction and by more effectively quantifying yield sensitivity to drought. More details in [here](../research/crop_yields_zambia/).
 
 
### References

- Chaney, N. W., Metcalfe, P., & Wood, E. F. (2016). HydroBlocks: a field-scale resolving land surface model for application over continental extents. Hydrological Processes. https://doi.org/10.1002/hyp.10891 

- Chaney, N. W., Torres-Rojas, L., Vergopolan, N., & Fisher, C. K. (2020). Two-way coupling between the sub-grid land surface and river networks in Earth system models. Geoscientific Model Development. https://doi.org/10.5194/gmd-2020-291

- Vergopolan, N., Chaney, N. W., Beck, H. E., Pan, M., Sheffield, J., Chan, S., & Wood, E. F. (2020). Combining hyper-resolution land surface modeling with SMAP brightness temperatures to obtain 30-m soil moisture estimates. Remote Sensing of Environment. https://doi.org/10.1016/j.rse.2020.111740

- Vergopolan, N., Xiong, S., Estes, L., Wanders, N., Chaney, N. W., Wood, E. F., Konar, M., Caylor, K., Beck, H. E., Gatti, N., Evans, T., & Sheffield, J. (2021). Field-scale soil moisture bridges the spatial-scale gap between drought monitoring and agricultural yields. Hydrology and Earth System Sciences. https://doi.org/10.5194/hess-25-1827-2021

