---
reading_time: true
commentable: false
date: "2020-12-31T00:00:00+01:00"
draft: true
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

HydroBlocks, a hyper-resolution land surface model that leverages the repeating spatial patterns over the landscape by implementing a hierarchical clustering algorithm to define its mesh ([Chaney et al., 2020](../publication/2020_chaney_two_way_coupling)). HydroBlocks groups the fine-scale drivers of the landscape spatial heterogeneity (e.g., 30-m land cover, soil properties, topography data) into complex tiles/clusters of similar hydrologic behavior. In this way, by simulating hydrological processes with clusters instead of regular grids, HydroBlocks yields an effective 30-m spatial resolution while leveraging the complex physics of land surface models and reducing the system's dimensionality and computational requirements.

HydroBlocks is a field-scale resolving land surface model that accounts for the water, energy, and carbon balance to solve land surface processes at high spatial and temporal resolutions. To define the computational mesh, HydroBlocks leverages the repeating patterns that exist over the landscape (i.e., the spatial organization) by clustering areas of assumed similar hydrologic behavior into HRUs. The simulation of these HRUs and their spatial interactions allows the modeling of hydrological, geophysical, and biophysical processes at the field scale (e.g., 30 m) over regional to continental extents (Chaney et al., 2016). 

The core of HydroBlocks is the Noah-MP vertical land surface scheme (Niu et al., 2011). HydroBlocks applies Noah-MP in an HRU framework to explicitly represent the spatial heterogeneity of surface processes down to field scale. At each time step, the land surface scheme updates the hydrological states at each HRU; and the HRUs dynamically interact laterally via surface and subsurface flow. In this way, HydroBlocks allows for the representation of water, energy, and carbon fluxes, as well as vegetation dynamics, accounted for in Noah-MP model.

To compute the subsurIn the original HydroBlocks, subsurface flow between HRUs was modeled via a subsurface kinematic wave. In this implementation, following the approach used in Chaney et al. (2018), the subsurface flow module has been updated by computing the Darcy flux between adjacent HRUs at each subsurface level. The fluxes are then included as divergence terms within their corresponding subsurface level of the vertical one-dimensional solution of Richards’ equation in Noah-MP. This allows for the flow of water between HRUs to also be driven by capillarity and not just the predefined topographic gradient. 

through out my Phd I have contributed to the development of HydroBlocks. In recent work, we 

I have been a developer for HydroBlocks, particularly what concerns 

## Applications on soil moisture simulations

The simulations in the header of this webpage demonstrates HydroBlocks capabilities for simulating 3-hourly soil moisture at an effective 30-m spatial resolution across the United States. In these simulations, we can observe that the soil moisture variability is mostly driven by the meteorological conditions, as the soil wets with the advance of the rainfall fronts. (point to the screen), but also driven by the landscape and topographic features. We can also observe the impacts of snow events on the soil moisture dynamics. The snow comes from the northern latitudes, and it melts either naturally or after a rain event. The soil moisture also changes throughout the season. As we approach the summer, the soil starts to dry drastically, especially in the southwest part of the country. 
At different locations, we can observe the impact of different soil properties in the soil moisture memory. For instance, in Florida, the exceptionally high sandy content leads to drier soil moisture conditions at the topsoil layer and very short soil moisture memory. This contrasts well with the soils from the Mississippi basins, which mostly comprise of silt and clay. 


Insets of this simulations are also ilustrated in Figure X and Y. 

{{< figure src="simualtions2.png" caption="" numbered="true" >}}
{{< figure src="slide2.png" caption="" numbered="true" >}}
{{< figure src="slide4b.png" caption="" numbered="true" >}}

## Towards assimilation of satellite observations

Our approach is built upon HydroBlocks, a hyper-resolution land surface model that leverages the repeating spatial patterns over the landscape by implementing a hierarchical clustering algorithm to define its mesh ([Chaney et al., 2020](../publication/2020_chaney_two_way_coupling)). HydroBlocks groups the fine-scale drivers of the landscape spatial heterogeneity (e.g., 30-m land cover, soil properties, topography data) into complex tiles/clusters of similar hydrologic behavior. In this way, by simulating hydrological processes with clusters instead of regular grids, HydroBlocks yields an effective 30-m spatial resolution while leveraging the complex physics of land surface models and reducing the system's dimensionality and computational requirements.

## Applications on crop yield modeling and prediction

To develop the SMAP-HydroBlocks dataset, we coupled HydroBlocks model with a Tau-Omega Radiative Transfer Model (HydroBlocks-RTM) to simulate the soil surface brightness temperature, and we merged it with the NASA's Soil Moisture Active-Passive (SMAP) L3 Enhanced 9-km brightness temperature product ([SMAP L3E](https://nsidc.org/data/SPL3SMP_E/versions/3)). For merging cluster-based model and grid-based satellite data we developed a cluster-based spatial Bayesian scheme ([Vergopolan et al., 2020](../publication/2020_vergopolan_combining)). We parameterized this merging scheme by regionalizing relationships extracted from satellite, models, and in-situ soil moisture observations using machine learning (Vergopolan et al., in review). With the fused brightness temperature, the inverse HydroBlocks-RTM model was applied to retrieve the SMAP-HydroBlocks (SMAP-HB) soil moisture estimates.

## Future Research


## Model availability
The HydroBlocks land surface model is available at [Github](https://github.com/chaneyn/HydroBlocks). 

## References

Chaney, N. W., Metcalfe, P. and Wood, E. F. *HydroBlocks: a field-scale resolving land surface model for application over continental extents*, Hydrol. Process., 30(20), https://doi.org/10.1002/hyp.10891, 2016.

Chaney, N. W., Torres-Rojas, L., Vergopolan, N., Fisher, C. K. *HydroBlocks v0.2: Enabling a field-scale two-way coupling between the land surface and river networks in Earth system models*. [In review](https://gmd.copernicus.org/preprints/gmd-2020-291/).


