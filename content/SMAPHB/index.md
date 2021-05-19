---
reading_time: true
commentable: false
date: "2021-04-16T00:00:00+01:00"
draft: false
editable: false
image:
  placement: 1
  caption: ''
  focal_point: 'center'
  preview_only: yes
header:
  image: "SMAPHB/header.png"
  caption: ""
tags:
- Soil Moisture
- Hyper-resolution
- Satellite
- HydroBlocks
share: true
title: "SMAP-HydroBlocks"
summary: The first hyper-resolution satellite-based surface soil moisture dataset at 30-m resolution over the continental United States
type: "page"
url: "SMAPHB/"

# Shortcodes - to add various content to the webpage
# https://gohugo.io/content-management/shortcodes
---

## Hyper-resolution satellite-based surface soil moisture over the continental United States

SMAP-HydroBlocks is a hyper-resolution satellite-based surface soil moisture product at 3-hourly 30-m resolution over the continental United States (2015-2019). This dataset combines microwave satellite remote sensing, hyper-resolution land surface model, radiative transfer modeling, machine learning, and in-situ observations to obtain hydrologically consistent soil moisture estimates of the top 5-cm of the soil.

Our approach is built upon HydroBlocks, a hyper-resolution land surface model that leverages the repeating spatial patterns over the landscape by implementing a hierarchical clustering algorithm to define its mesh ([Chaney et al., 2020](../publication/2020_chaney_two_way_coupling)). HydroBlocks groups the fine-scale drivers of the landscape spatial heterogeneity (e.g., 30-m land cover, soil properties, topography data) into complex tiles/clusters of similar hydrologic behavior. In this way, by simulating hydrological processes with clusters instead of regular grids, HydroBlocks yields an effective 30-m spatial resolution while leveraging the complex physics of land surface models and reducing the system's dimensionality and computational requirements.

To develop the SMAP-HydroBlocks dataset, we coupled HydroBlocks model with a Tau-Omega Radiative Transfer Model (HydroBlocks-RTM) to simulate the soil surface brightness temperature, and we merged it with the NASA's Soil Moisture Active-Passive (SMAP) L3 Enhanced 9-km brightness temperature product ([SMAP L3E](https://nsidc.org/data/SPL3SMP_E/versions/3)). For merging cluster-based model and grid-based satellite data we developed a cluster-based spatial Bayesian scheme ([Vergopolan et al., 2020](../publication/2020_vergopolan_combining)). We parameterized this merging scheme by regionalizing relationships extracted from satellite, models, and in-situ soil moisture observations using machine learning (Vergopolan et al., in review). With the fused brightness temperature, the inverse HydroBlocks-RTM model was applied to retrieve the SMAP-HydroBlocks (SMAP-HB) soil moisture estimates.

For illustration, SMAP-HB long-term and annual climatology at 30-m resolution is shown in the Soil Moisture Visualization tab.

<div style="text-align: center;">
{{% staticref "https://smaphbvis3.waterai.earth/" "newtab" %}}Open Fullscreen{{% /staticref %}}
</div>


<div class='visualizer' style="position: relative; padding-bottom: 100%; width: 100%; height: 120%; overflow: hidden;">
  <iframe scrolling="no" src="https://smaphbvis5.waterai.earth/" style="position:absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; margin-top: -102px; " allowfullscreen='true' webkitallowfullscreen='true' mozallowfullscreen='true' allowvr="yes"></iframe>
</div>



#### Data availability
Subsets of the SMAP-HB dataset at 30-m 3-hr resolution (2015–2019) are available on request. An aggregated version of the SMAP-HB dataset at 1-km 6-hr resolution (2015–2019) is available for download [here](https://zenodo.org/record/4441212).

#### Data citation
Please cite the following paper when using the dataset in any publication:

Vergopolan, N., Chaney, N. W., Beck, H. E., Pan, M., Sheffield, J., Chan, S., & Wood, E. F. (2020). Combining hyper-resolution land surface modeling with SMAP brightness temperatures to obtain 30-m soil moisture estimates. Remote Sensing of Environment, 242, 111740. https://doi.org/10.1016/j.rse.2020.111740
