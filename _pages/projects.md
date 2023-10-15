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

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/particle.gif" style="float:right; width: 50%; height: 50%">

Lagrangian particle tracking is widely utilized to study transport features in oceanography. In this study, we officially introduced a new offline particle tracking package, [Tracker](https://github.com/parkermac/LO/tree/main/tracker), and evaluated its performance in comparison to ROMS online dye and online particle tracking ([floats](https://www.myroms.org/wiki/floats.in)), and three offline particle tracking software packages ([LTRANS](https://northweb.hpl.umces.edu/LTRANS.htm), [OpenDrift](https://opendrift.github.io/), [Particulator](https://github.com/neilbanas/particulator)). It was found that both particle and dye approaches gave similar results across different model resolutions and domains when they were tracking the same water mass. The flexibility of offline particle tracking and its similarity against online dye and particle tracking make it a useful tool to complement existing ocean circulation models. The new Tracker was shown to be a reliable particle tracking package to complement ROMS. We also explored the tradeoffs of computational efficiency, modifiability, and ease of use that can influence the choice of which package. The main value of the present study is that the different particle and dye tracking codes were all run on the same model output, or within the model that generated the output. This allows some measure of intercomparison of the different tracking schemes.

Publication:

Xiong, J., MacCready, P. Intercomparisons of five ocean particle tracking software packages in the Regional Ocean Modeling System. Geoscientific Model Development ([in review](https://gmd.copernicus.org/preprints/gmd-2023-45/gmd-2023-45.pdf)).


**Development of a biophysical model to simulate harmful algal bloom in Chesapeake Bay**

Harmful algal blooms (HABs) threaten marine life and human health. Lagrangian particle tracking (LPT) is a popular tool to track algal blooms, yet most LPT models use passive numerical particles to represent algae without considering their interactions with ambient environments, including water temperature, salinity, available light, and nutrient concentrations. To advance predictions of HABs, we developed a new LPT-Biological (LPT-Bio) model that integrates the advantages of both Lagrangian and Eulerian 
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/LPT_Bio_model.jpg" style="float:right; width: 60%; height: 60%">
approaches. We included algal dynamics (mixotrophic growth, respiration, and mortality) and diel vertical migration to numerical particles based on the modeling system SCHISM. The improved LPT-Bio model was applied to simulate the 2020 [Margalefidinium polykrikoides](https://www.vims.edu/bayinfo/habs/guide/cochlodinium.php) bloom in Chesapeake Bay and successfully captured bloom intensity, duration, spatial extent, and resolved locally aggregated patchiness. We found that capturing DVM patterns and including mixotrophic growth are critical for HAB simulation. The present model framework can provide a basis for developing a forecast system for HABs in the Bay.

The LPT-Bio model is further used to investigate mechanisms of the coastward expansion of M. polykrikoides in the summer of 2020 after a tropical storm passed the Bay. Such coastward expansion was only recorded in 2007. We found that the persistent pre-storm southerly winds favored the delivery of bloom source water (originated inside the bay) to the coast. Storm-induced strong upwelling of denser subsurface water interacted with the after-storm outflow plume, forming a transport barrier to accumulate algae and delineate the coastwide bloom extent. Algal diel vertical migrations and transport barrier enable algae to stay in the nearshore regions. The storm-induced coastward expansion of M. polykrikoides might increase future bloom possibilities in the coastal area.

Publication:

Xiong, J., Shen, J., Qin, Q., Tomlinson, M. C., Zhang, Y. J., Cai, X., Ye, F., Cui, L., Mulholland, M. R. (2023). Biophysical interactions control the progression of harmful algal blooms in Chesapeake Bay: a novel Lagrangian particle tracking model with mixotrophic growth and vertical migration. [Limnology and Oceanography Letters](https://aslopubs.onlinelibrary.wiley.com/doi/full/10.1002/lol2.10308).

Xiong, J., Shen, J., Wang, Q. (2022). Storm-induced coastward expansion of Margalefidinium polykrikides in Chesapeake Bay. [Marine Pollution Bulletin, 184, 114187](https://www.sciencedirect.com/science/article/abs/pii/S0025326X22008694).

**Long-term variabilities (32 years) of exchange flow and reflux-efflux in Chesapeake Bay**
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/TEF_Illustration_v4.jpg" style="float:right; width: 60%; height: 60%">
Water exchange, featured by bottom inflow and surface outflow in a typical estuary, determines the transport and redistribution of salt, nutrients, pollutants, and suspended sediments and organisms. Based on a long-term (1980–2011) numerical model simulation, this study examines the water exchanges between Chesapeake Bay and the adjacent coastal shelf, and between different regions within the bay. Through an EOF analysis, we found that over 90% of the spatiotemporal variations of water exchange can be explained by freshwater discharge and northwesterly wind. Unlike the outflow that increases linearly with river discharge as commonly expected, the inflow initially increases with river discharge due to enhanced gravitational circulation and then levels, and gradually declines due to overwhelming seaward barotropic current. A locally enhanced water exchange was found in the lower-middle bay, associated with the persistent reflux (quantified using [TEF](https://github.com/parkermac/LO/tree/main/extract/tef2)) of surface outflow due to the shoaling of the main channel (i.e. Rappahannock Shoal near the mouth). 

Publication:

Xiong, J., Shen, J., Qin, Q. (2021). Exchange flow and material transport along the salinity gradient in a long estuary. [Journal of Geophysical Research: Oceans, e2021JC017185](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021JC017185).

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. [Journal of Marine Systems, 103497](https://www.sciencedirect.com/science/article/abs/pii/S0924796320301925).

**Application of transport timescales in Chesapeake Bay**

The hydrodynamics-regulated transport process can be quantitatively described using a transport timescale. A wealth of terminologies related to transport timescale has been used in the literatures since the seminal work on diagnostic timescale by Bolin & Rodhe (1973), including residence time, partial residence time, flushing time, exposure time, transit time, water age, partial age, influence time, renewal time, etc. 
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/definition.png" style="float:right; width: 60%; height: 60%">. Transport timescale provides a 4th-dimensional time information to distill the details of hydrodynamic circulations and acts as a common currency to compare the physical transport time with the timescale for biochemical reactions. 

With valid definitions, transport timescale can be tailored to serve various study purposes. For example, by adjusting the location of boundaries where the material (or water parcel) exits, residence time (no return) in different segments of Chesapeake Bay can be quantified; by controlling whether the exited materials return or not, the transport time was termed as “exposure time”, which can be used to quantify the total time for nutrients or pollutants to stay in an area of interest; by comparing residence time and exposure time, a retention coefficient can be calculated to quantify the material retention efficiency; by controlling the virtual clock attached to each (sinking) particle (or water parcel), the time spent in different subregions (e.g., water column and bottom sediments) along the transport trajectories can be quantified; 


The water exchange and the mean residence time can be connected reciprocally through the bay volume, yet the validation of this relationship depends on the timescale to be considered since the residence time at a given time is controlled by the future hydrodynamics. A delay effect should be considered when using the relationship to estimate outflow interchangeably with the direct computation of the outflow.

Publication:

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. [Journal of Marine Systems, 103497](https://www.sciencedirect.com/science/article/abs/pii/S0924796320301925).

Xiong, J., Shen, J. (2022). Vertical transport timescale of surface-produced particulate material in the Chesapeake Bay. [Journal of Geophysical Research: Oceans, e2021JC017592](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021JC017592).

**Mechanisms of high suspended sediment concentration in the southern Yellow Sea, China**

An understanding of the dynamics and behaviors of suspended sediments is vital in analysis of 
morphological, environmental, and ecological processes occurring in coastal marine environments. To 
study the mechanisms of maintaining high suspended sediment concentrations (SSCs) on a tide-dominated 
offshore shoal, we measured water depths, current velocities, SSCs, wave parameters and bottom sediment 
compositions in the southern Yellow Sea. These data were then used to calculate bottom shear stresses 
generated by currents (tc), waves (tw), and wave-current interactions (tcw). SSCs time series exhibited 
strong quarter-diurnal peaks during spring tides, in contrast to the semidiurnal signal during neap 
tides. A Fourier analysis showed that suspended sediment variations within tidal cycles was mainly 
controlled by resuspension in most stations. There existed relatively stable background SSCs 
(maintaining high SSCs among tidal cycles) values at all four stations during both windy (wind speed > 
9.0 m/s) and normal weather conditions (wind speed < 3.0 m/s). The background SSCs had strong 
relationship with spring/neap-averaged tcw, indicating background SSCs were mainly controlled by mean 
bottom shear stress, with a minimum value of 0.21 N/m2. On account of the strong tidal cur- rents, 
background SSCs of spring tides were greater than that of neap tides. In addition, on the base of 
wavelet, statistics analyses and turbulence dissipation parameter, background SSCs during slack tide in 
the study area may be maintained by intermittent turbulence events induced by a combined tidal current 
and wave action.

Publication: 

Xiong, J., Wang, X. H., Wang, Y. P., Chen, J., Shi, B., Gao, J., Yang, Y., Yu, Q., Li, M., Yang, L., Gong, X. (2017). Mechanisms of maintaining high suspended sediment concentration over tide-dominated offshore shoals in the Southern Yellow Sea. [Estuarine, Coastal and Shelf Science, 191, 221-233](https://www.sciencedirect.com/science/article/abs/pii/S0272771417304389).

**wave dynamics**

Publication:

Xiong, J., You, Z., Li, J., Gao, S., Wang, Q., Wang, Y. P. (2020). Variations of wave parameter statistics as influenced by water depth in coastal and shelf areas. [Coastal Engineering, 103717](https://www.sciencedirect.com/science/article/abs/pii/S0378383919303679).

Xiong, J., Wang, Y. P., Gao, S., Du, J., Yang, Y. (2018). On estimation of coastal wave parameters and wave-induced shear stress. [Limnology and Oceanography: Methods, 16(9): 594-606](https://aslopubs.onlinelibrary.wiley.com/doi/full/10.1002/lom3.10271).

