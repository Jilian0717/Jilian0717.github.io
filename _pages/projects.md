---
layout: page
title: research
permalink: /projects/
description: I'm mainly using oceanographic numerical models, Lagrangian particle tracking, and the concept of transport timescales to study how physics impacts the transport and fate of estuarine and coastal materials (nutrients, particulates, swimming algae, sediments...). During my master's, I analyzed coastal wave dynamics and high suspended sediment concentrations based on observations.
nav: true
nav_order: 1
display_categories: []
horizontal: true
---
<span style="text-decoration: underline">Selected projects:</span>

**Intercomparison of Lagrangian particle tracking software packages in ROMS**

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/particle.gif" style="float:right; width: 50%; height: 50%">

Lagrangian particle tracking is widely utilized to study transport features in oceanography. In this study, we officially introduced a new offline particle tracking package, [Tracker](https://github.com/parkermac/LO/tree/main/tracker), and evaluated its performance in comparison to ROMS online dye and online particle tracking ([floats](https://www.myroms.org/wiki/floats.in)), and three offline particle tracking software packages ([LTRANS](https://northweb.hpl.umces.edu/LTRANS.htm), [OpenDrift](https://opendrift.github.io/), [Particulator](https://github.com/neilbanas/particulator)). It was found that both particle and dye approaches gave similar results across different model resolutions and domains when they were tracking the same water mass. The flexibility of offline particle tracking and its similarity against online dye and particle tracking make it a useful tool to complement existing ocean circulation models. The new Tracker was shown to be a reliable particle tracking package to complement ROMS. We also explored the tradeoffs of computational efficiency, modifiability, and ease of use that can influence the choice of which package. The main value of the present study is that the different particle and dye tracking codes were all run on the same model output, or within the model that generated the output. This allows some measure of intercomparison of the different tracking schemes.

Publication:

Xiong, J., & MacCready, P. (2024). Intercomparisons of Tracker v1.1 and four other ocean particle-tracking software packages in the Regional Ocean Modeling System. [Geoscientific Model Development, 17(8), 3341-3356](https://gmd.copernicus.org/articles/17/3341/2024/).


**Developing a biophysical model to simulate harmful algal bloom in Chesapeake Bay**

Harmful algal blooms (HABs) threaten marine life and human health. Lagrangian particle tracking (LPT) is a popular tool to track algal blooms, yet most LPT models use passive numerical particles to represent algae without considering their interactions with ambient environments, including water temperature, salinity, available light, and nutrient concentrations. To advance predictions of HABs, we developed a new LPT-Biological (LPT-Bio) model that integrates the advantages of both Lagrangian and Eulerian 
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/LPT_Bio_model.jpg" style="float:right; width: 60%; height: 60%">
approaches. We included algal dynamics (mixotrophic growth, respiration, and mortality) and diel vertical migration to numerical particles based on the modeling system SCHISM. The improved LPT-Bio model was applied to simulate the 2020 [Margalefidinium polykrikoides](https://www.vims.edu/bayinfo/habs/guide/cochlodinium.php) bloom in Chesapeake Bay and successfully captured bloom intensity, duration, spatial extent, and resolved locally aggregated patchiness. We found that capturing DVM patterns and including mixotrophic growth are critical for HAB simulation. The present model framework can provide a basis for developing a forecast system for HABs in the Bay.

The LPT-Bio model is further used to investigate mechanisms of the coastward expansion of *M. polykrikoides* in the summer of 2020 after a tropical storm passed the Bay. Such coastward expansion was only recorded in 2007. We found that the persistent pre-storm southerly winds favored the delivery of bloom source water (originated inside the bay) to the coast. Storm-induced strong upwelling of denser subsurface water interacted with the after-storm outflow plume, forming a transport barrier to accumulate algae and delineate the coastwide bloom extent. Algal diel vertical migrations and transport barrier enable algae to stay in the nearshore regions. The storm-induced coastward expansion of *M. polykrikoides* might increase future bloom possibilities in the coastal area.

Publication:

Xiong, J., Shen, J., Qin, Q., Tomlinson, M. C., Zhang, Y. J., Cai, X., Ye, F., Cui, L., Mulholland, M. R. (2023). Biophysical interactions control the progression of harmful algal blooms in Chesapeake Bay: a novel Lagrangian particle tracking model with mixotrophic growth and vertical migration. [Limnology and Oceanography Letters](https://aslopubs.onlinelibrary.wiley.com/doi/full/10.1002/lol2.10308). Selected as VIMS Best Student Paper [Awards](https://www.vims.edu/newsandevents/topstories/2023/student_awards/best_student_paper.php), 2023.

Xiong, J., Shen, J., Wang, Q. (2022). Storm-induced coastward expansion of Margalefidinium polykrikides in Chesapeake Bay. [Marine Pollution Bulletin, 184, 114187](https://www.sciencedirect.com/science/article/abs/pii/S0025326X22008694).


**Exchange flow and water reflux-efflux in Chesapeake Bay**
<img class="col one last" src="{{ site.baseurl}}/assets/img/publication_preview/TEF_Illustration_v4.jpg" style="float:right; width: 60%; height: 60%">

Water exchange, featured by bottom inflow and surface outflow in a typical estuary, determines the transport and redistribution of salt, nutrients, pollutants, and suspended sediments and organisms. Based on a long-term (1980–2011) numerical model simulation, this study examines the water exchanges between Chesapeake Bay and the adjacent coastal shelf, and between different regions within the bay. Through an EOF analysis, we found that over 90% of the spatiotemporal variations of water exchange can be explained by freshwater discharge and northwesterly wind. Unlike the outflow that increases linearly with river discharge as commonly expected, the inflow initially increases with river discharge due to enhanced gravitational circulation and then levels, and gradually declines due to overwhelming seaward barotropic current. A locally enhanced water exchange was found in the lower-middle bay, associated with the persistent reflux (quantified using [TEF](https://github.com/parkermac/LO/tree/main/extract/tef2)) of surface outflow due to the shoaling of the main channel (i.e. Rappahannock Shoal near the mouth). 

Publication:

Xiong, J., Shen, J., Qin, Q. (2021). Exchange flow and material transport along the salinity gradient in a long estuary. [Journal of Geophysical Research: Oceans, e2021JC017185](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021JC017185).

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. [Journal of Marine Systems, 103497](https://www.sciencedirect.com/science/article/abs/pii/S0924796320301925).


**Applications of transport timescales in Chesapeake Bay**

Transport timescale provides 4th-dimensional time information to distill the details of hydrodynamic circulations and acts as a common currency to compare the physical transport time with the timescale for biochemical reactions. A wealth of terminologies related to transport timescales have been used in the literature since the seminal work on diagnostic timescale by Bolin & Rodhe (1973): residence time, partial residence time, flushing time, exposure time, transit time, water age, partial age, influence time, renewal time, etc. 

With valid definitions, the transport timescale can be tailored to serve various study purposes. For example:
<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/definition.png" style="float:right; width: 60%; height: 60%">
- by adjusting the boundary where the material (or water parcel) exits for the first time, residence time in different subdomains can be quantified.
- by counting the subsequent material (or water) re-entering, the transport timescale can be termed as “exposure time”, which quantifies the total time for nutrients or pollutants to stay in an area of interest.
- by comparing residence time and exposure time, a retention coefficient can be calculated to quantify the material retention efficiency.
- by controlling a virtual clock⏰ attached to each (sinking) particle (or water parcel), the time spent in different subregions (e.g., water column and bottom sediments) along the transport trajectories can be quantified.

Publication:

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. [Journal of Marine Systems, 103497](https://www.sciencedirect.com/science/article/abs/pii/S0924796320301925).

Xiong, J., Shen, J. (2022). Vertical transport timescale of surface-produced particulate material in the Chesapeake Bay. [Journal of Geophysical Research: Oceans, e2021JC017592](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021JC017592).


**Mechanisms of high suspended sediment concentration in the southern Yellow Sea, China**

Understanding the dynamics and behaviors of suspended sediments is vital for analyzing the morphological, environmental, and ecological processes in coastal environments. To study the mechanisms 
<img class="col one last" src="{{ site.baseurl}}/assets/img/publication_preview/background_ssc.png" style="float:right; width: 50%; height: 50%"> of the high suspended sediment concentrations (SSCs > 1 kg/m<sup>3</sup>) in a tidally dominated offshore shoal in the southern Yellow Sea, we measured water depths, current velocities, SSCs, wave parameters, and bottom sediment compositions from 27 September to 5 October 2014 via near-bed tripod systems. The SSCs time series exhibited strong semidiurnal peaks during the neap tide, in contrast to the quarter-diurnal signal during the spring tide. Based on a Fourier analysis, M4 component of SSCs (due to resuspension) controls the variations of the high SSC in most sites. A relatively constant high background SSC was also identified in the study area. The maintenance of the background SSCs during the slack tides may due to the intermittent turbulence that was driven by a combined tidal current and wave action.

Publication: 

Xiong, J., Wang, X. H., Wang, Y. P., Chen, J., Shi, B., Gao, J., Yang, Y., Yu, Q., Li, M., Yang, L., Gong, X. (2017). Mechanisms of maintaining high suspended sediment concentration over tide-dominated offshore shoals in the Southern Yellow Sea. [Estuarine, Coastal and Shelf Science, 191, 221-233](https://www.sciencedirect.com/science/article/abs/pii/S0272771417304389).


**Wave🌊 parameters and wave-induced shear stress**

Wave parameters, e.g., wave height, near-bed wave orbital velocity, and wave-induced shear stresses, are important hydrodynamic parameters for sediment processes in coastal oceans and also useful in designing coastal structures to assess the safety of offshore platforms. Wave orbital velocity is particularly critical in sediment resuspension. Several algorithms to calculate <img class="col one last" src="{{ site.baseurl}}/assets/img/publication_preview/Uw_turbulence.png" style="float:right; width: 60%; height: 60%"> wave orbital velocity have been proposed, including linear wave theory, spectrum, and Joint North Sea Wave Project methods, but the validity of these algorithms in relatively shallow waters is not well understood. In this study, we compared the wave parameters obtained by different instruments and algorithms at four sites, one within the intertidal zone with a mean depth of 1 m and the other three in deeper offshore water with mean depths of 15–30 m. We found a high consistency of the estimated wave height, peak wave period, and wave orbital velocity among different datasets and different algorithms at the offshore sites, while there were significant discrepancies at the shoreline site. Using Ursell number, our study suggests that it is reliable to apply any of the three algorithms and different instruments (acoustic Doppler velocimeter and buoy) in deeper water. However, for very shallow water, it is recommended to use the measured high-frequent velocity and spectrum method to calculate wave orbital velocity and use a wave gauge instrument or zero-crossing algorithm to obtain wave height and period information. Finally, the effect of turbulence and bed-form morphology on wave-induced shear stress is discussed: without removing the turbulence or taking into account bedforms (e.g., ripples), the orbital velocity will be remarkably over-estimated or under-estimated.

In addition, the statistics of wave parameters at different water depths are analyzed. The frequencies of occurrence distributions of wave pressure amplitude P and orbital velocity amplitude U are compared with the three commonly used, classic Rayleigh, modified Rayleigh, and Weibull distributions. It is found that the distribution of P is almost identical to that of U for each site. The distributions of P and U for the intertidal flat sites fit the Weibull distribution better than the classic or modified Rayleigh ones, indicating a shallowness effect that is associated with finite-banded wind-wave spectra and possible wave breaking or near-bed turbulence. On the other hand, the distributions of P and U measured at the three inner shelf sites agree almost equally with the three distributions. With increasing water depth, the distributions of P and U are shown to reduce from the two-parameter Weibull distribution at the shallow intertidal sites to the classic Rayleigh at the deep-water sites. For coastal engineering applications, an empirical formula is proposed to estimate more accurately the significant wave height in intermediate coastal waters based on the surface water elevation data.

Publication:

Xiong, J., You, Z., Li, J., Gao, S., Wang, Q., Wang, Y. P. (2020). Variations of wave parameter statistics as influenced by water depth in coastal and shelf areas. [Coastal Engineering, 103717](https://www.sciencedirect.com/science/article/abs/pii/S0378383919303679).

Xiong, J., Wang, Y. P., Gao, S., Du, J., Yang, Y. (2018). On estimation of coastal wave parameters and wave-induced shear stress. [Limnology and Oceanography: Methods, 16(9): 594-606](https://aslopubs.onlinelibrary.wiley.com/doi/full/10.1002/lom3.10271).

An [article](https://sgos.nju.edu.cn/cb/0f/c8418a641807/page.htm) (in Chinese) introducing research on waves in Dr. Ya Ping Wang's group at Nanjing University.
