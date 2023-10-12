---
layout: page
title: research
permalink: /projects/
description: I use oceanographic numerical models, Lagrangian particle tracking, and the concept of transport timescales to study what does physics do to the transport and fate of estuarine/coastal materials
nav: true
nav_order: 1
display_categories: []
horizontal: false
---
<span style="text-decoration: underline">Selected projects:</span>

**Intercomparison of Lagrangian particle tracking software packages in ROMS**

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/particle.gif" style="float:right; width: 40%; height: 40%">

Lagrangian particle tracking is widely utilized to study transport features in oceanography. In this study, we officially introduced a new offline particle tracking package, [Tracker](https://github.com/parkermac/LO/tree/main/tracker), and evaluated its performance in comparison to ROMS online dye and online particle tracking ([floats](https://www.myroms.org/wiki/floats.in)), and three offline particle tracking software packages ([LTRANS](https://northweb.hpl.umces.edu/LTRANS.htm), [OpenDrift](https://opendrift.github.io/), [Particulator](https://github.com/neilbanas/particulator)). It was found that both particle and dye approaches gave similar results across different model resolutions and domains when they were tracking the same water mass. The flexibility of offline particle tracking and its similarity against online dye and particle tracking make it a useful tool to complement existing ocean circulation models. The new Tracker was shown to be a reliable particle tracking package to complement ROMS. We also explored the tradeoffs of computational efficiency, modifiability, and ease of use that can influence the choice of which package. The main value of the present study is that the different particle and dye tracking codes were all run on the same model output, or within the model that generated the output. This allows some measure of intercomparison of the different tracking schemes.

Publication:

Xiong, J., MacCready, P. Intercomparisons of five ocean particle tracking software packages in the Regional Ocean Modeling System. Geoscientific Model Development ([in review](https://gmd.copernicus.org/preprints/gmd-2023-45/gmd-2023-45.pdf)).


**Development of a biophysical model to simulate harmful algal bloom in Chesapeake Bay**

Harmful algal blooms (HABs) threaten marine life and human health. Lagrangian particle tracking (LPT) is a popular tool to track algal blooms, yet most LPT models use passive numerical particles to represent algae without considering their interactions with ambient environments, including water temperature, salinity, available light, and nutrient concentrations. To advance predictions of HABs, we developed a new LPT-Biological (LPT-Bio) model that integrates the advantages of both Lagrangian and Eulerian 
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/LPT_Bio_model.jpg" style="float:right; width: 60%; height: 60%">
approaches. We included algal dynamics (mixotrophic growth, respiration, and mortality) and diel vertical migration to numerical particles based on the modeling system SCHISM. The improved LPT-Bio model was applied to simulate the 2020 [Margalefidinium polykrikoides](https://www.vims.edu/bayinfo/habs/guide/cochlodinium.php) bloom in Chesapeake Bay and successfully captured bloom intensity, duration, spatial extent, and resolved locally aggregated patchiness. We found that capturing DVM patterns and including mixotrophic growth are critical for HAB simulation. The present model framework can provide a basis for developing a forecast system for HABs in the Bay.

The LPT-Bio model is further used to investigate mechanisms of the coastward expansion of M. polykrikoides in the summer of 2020 after a tropical storm passed the Bay. Such coastward expansion was only recorded in 2007. We found that the persistent pre-storm southerly winds favored the delivery of bloom source water (originated inside the bay) to the coast. Storm-induced strong upwelling of denser subsurface water interacted with the after-storm outflow plume, forming a transport barrier to accumulate algae and delineate the coastwide bloom extent. Algal diel vertical migrations and transport barrier enable algae to stay in the nearshore regions. The storm-induced coastward expansion of M. polykrikoides might increase future bloom possibilities in the coastal area.

Publication:

Xiong, J., Shen, J., Qin, Q., Tomlinson, M. C., Zhang, Y. J., Cai, X., Ye, F., Cui, L., Mulholland, M. R. (2023). Biophysical interactions control the progression of harmful algal blooms in Chesapeake Bay: a novel Lagrangian particle tracking model with mixotrophic growth and vertical migration. Limnology and Oceanography Letters.

Xiong, J., Shen, J., Wang, Q. (2022). Storm-induced coastward expansion of Margalefidinium polykrikides in Chesapeake Bay. Marine Pollution Bulletin, 184, 114187.

**Long-term variabilities (32 years) of exchange flow and reflux-efflux in Chesapeake Bay**

Water exchange, featured by bottom inflow and surface outflow in a typical estuary, determines the transport and redistribution of salt, nutrients, pollutants, and suspended sediments and organisms. Based on a long-term (1980–2011) numerical model simulation, this study examines the water exchanges between Chesapeake Bay and the adjacent coastal shelf, and between different regions within the bay. Through an EOF analysis, we found that over 90% of the spatiotemporal variations of water exchange can be explained by freshwater discharge and northwesterly wind. Unlike the outflow that increases linearly with river discharge as commonly expected, the inflow initially increases with river discharge due to enhanced gravitational circulation and then levels, and gradually declines due to overwhelming seaward barotropic current. A locally enhanced water exchange was found in the lower-middle bay, associated with the persistent reflux (quantified using [TEF](https://github.com/parkermac/LO/tree/main/extract/tef2)) of surface outflow due to the shoaling of the main channel (i.e. Rappahannock Shoal near the mouth). 
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/TEF_Illustration_v4.jpg" style="float:center; width: 40%; height: 40%">

Publication:

Xiong, J., Shen, J., Qin, Q. (2021). Exchange flow and material transport along the salinity gradient in a long estuary. Journal of Geophysical Research: Oceans, e2021JC017185.

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. Journal of Marine Systems, 103497.

**Transport timescale of riverine dissolved material and surface-produced particulates in Chesapeake Bay**

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/definition.png" style="float:center; width: 40%; height: 40%">

The water exchange and the mean residence time can be connected reciprocally through the bay volume, yet the validation of this relationship depends on the timescale to be considered since the residence time at a given time is controlled by the future hydrodynamics. A delay effect should be considered when using the relationship to estimate outflow interchangeably with the direct computation of the outflow.

A retention coefficient was adopted to quantify the material retention rate using two characteristic PRTs: with and without incorporating water parcels returning to a concerned region. It is found that shoaling from the Rappahannock Shoal to the mouth causes persistent downwelling, strong reflux, and the highest material retention rate in the middle of the bay. 

The accumulations of particulate organic matter (POM) produced from spring phytoplankton bloom in the bottom layer fuels summertime hypoxia in CB. We applied the vertical particulate age (VPA), the average time elapsed since the particulate organic matter leaves the surface water, to estimate the downward-transport time. The VPA accounts for all possible trajectories, including direct sinking and interactions with the seabed via resuspension and deposition. It was found that the VPA is much longer than the vertical transport time for dissolved material due to the elongated resting of particulates on the seabed and contributions from the resuspended old material. The VPA is sensitive to the settling velocity and increases 2 orders of magnitude with the settling velocity from 0 to 10 m/day in less dynamic environments. The slow-sinking material can remain in suspension while the fast-sinking material mostly stays on the seabed. No significant difference in the VPA was found between wet and dry years except during the episodic freshwater pulse, which brought aged materials from the depositional shoals to increase the VPA in the channel.


Publication:

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. Journal of Marine Systems, 103497.

Xiong, J., Shen, J. (2022). Vertical transport timescale of surface-produced particulate material in the Chesapeake Bay. Journal of Geophysical Research: Oceans, e2021JC017592.

**Mechanisms of high suspended sediment concentration in the southern Yellow Sea, China**

Publication: 

Xiong, J., Wang, X. H., Wang, Y. P., Chen, J., Shi, B., Gao, J., Yang, Y., Yu, Q., Li, M., Yang, L., Gong, X. (2017). Mechanisms of maintaining high suspended sediment concentration over tide-dominated offshore shoals in the Southern Yellow Sea. Estuarine, Coastal and Shelf Science, 191, 221-233.

**wave dynamics**

Publication:

Xiong, J., You, Z., Li, J., Gao, S., Wang, Q., Wang, Y. P. (2020). Variations of wave parameter statistics as influenced by water depth in coastal and shelf areas. Coastal Engineering, 103717.

Xiong, J., Wang, Y. P., Gao, S., Du, J., Yang, Y. (2018). On estimation of coastal wave parameters and wave-induced shear stress. Limnology and Oceanography: Methods, 16(9): 594-606.

