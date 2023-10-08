---
layout: page
title: projects
permalink: /projects/
description: I use oceanographic numerical models, Lagrangian particle tracking, and the concept of transport timescales to study what does physics do to the transport and fate of estuarine/coastal materials
nav: true
nav_order: 1
display_categories: []
horizontal: false
---
<span style="text-decoration: underline">Selected projects:</span>

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/particle.gif" style="float:right; width: 40%; height: 40%">

**Intercomparison of Lagrangian particle tracking software packages in ROMS**

Lagrangian particle tracking is widely utilized to study transport features in a range of physical, chemical, and biological processes in oceanography. In this study, we officially introduced a new offline particle tracking package, [Tracker](https://github.com/parkermac/LO/tree/main/tracker), and evaluted its performance in comparison to ROMS online dye and online particle tracking ([floats](https://www.myroms.org/wiki/floats.in)), and three offline particle tracking software packages ([LTRANS](https://northweb.hpl.umces.edu/LTRANS.htm), [OpenDrift](https://opendrift.github.io/), [Particulator](https://github.com/neilbanas/particulator)). It was found that both particle and dye approaches give similar results across different model resolutions and domains when they were tracking the same water mass, as indicated by similar mean advection pathways and spatial distributions of dye and particles. The flexibility of offline particle tracking and its similarity against online dye and particle tracking make it a useful tool to complement existing ocean circulation models. The new Tracker was shown to be a reliable particle tracking package to complement ROMS. Lastly, we also explored the tradeoffs of computational efficiency, modifiability, and ease of use that can influence the choice of which package. The main value of the present study is that the different particle and dye tracking codes were all run on the same model output, or within the model that generated the output. This allows some measure of intercomparison of the different tracking schemes.

publication:

Xiong, J., MacCready, P. Intercomparisons of five ocean particle tracking software packages in the Regional Ocean Modeling System. Geoscientific Model Development ([in review](https://gmd.copernicus.org/preprints/gmd-2023-45/gmd-2023-45.pdf)).


**Development of a biophysical model to simulate Margalefidinium Polykrikoides Bloom in Chesapeake Bay**

Harmful algal blooms (HABs) threaten human health, marine life, and coastal economies. Accurate prediction of HABs is still a challenge. Lagrangian particle tracking (LPT) is a popular tool to track algal blooms, yet most LPT models use passive particles to represent algae without considering their interactions with ambient environmental conditions, including water temperature, salinity, available light, and nutrient concentrations. To advance predictions of HABs, we developed a novel LPT-Biological (LPT-Bio) model that integrates the advantages of both Lagrangian and Eulerian approaches by incorporating algal dynamics (mixotrophic growth, respiration, and mortality), algal biomass change, and diel vertical migration (DVM), along the predicted transport trajectories. The model is fully controlled by environmental conditions while maintaining mass balance. The improved LPT-Bio model was applied to simulate the 2020 Margalefidinium polykrikoides bloom in the Chesapeake Bay and successfully captured bloom intensity/duration/spatial extent and resolved locally aggregated patchiness. We found that capturing DVM patterns and including mixotrophic growth are critical for HAB simulation. The present model framework can provide a basis for developing a forecast system for HABs in the Bay.

<img class="col one last" src="{{ site.baseurl }}/assets/img/publication_preview/HAB_simulation.png" style="float:right; width: 40%; height: 40%">

The LPT-Bio model is further used to investigate the underlying mechanisms of the coastward expansion of M. polykrikoides in 2020 summer after a tropical storm passing Chesapeake Bay. Such coastward expansion was only recorded in 2007. We found that the persistent pre-storm southerly winds favored the delivery of bloom source water originated inside the bay to the coast. Storm-induced strong upwelling of denser subsurface water interacted with the after-storm outflow plume (steered southward as the storm's impacts waned), forming a transport barrier to accumulate algae and delineate the coastwide bloom extent. Algal diel vertical migrations and transport barrier enable algae to stay in the nearshore regions. The storm-induced coastward expansion of M. polykrikoides might increase future bloom possibility in the coastal area.

Publication:

Xiong, J., Shen, J., Qin, Q., Tomlinson, M. C., Zhang, Y. J., Cai, X., Ye, F., Cui, L., Mulholland, M. R. (2023). Biophysical interactions control the progression of harmful algal blooms in Chesapeake Bay: a novel Lagrangian particle tracking model with mixotrophic growth and vertical migration. Limnology and Oceanography Letters.

Xiong, J., Shen, J., Wang, Q. (2022). Storm-induced coastward expansion of Margalefidinium polykrikides in Chesapeake Bay. Marine Pollution Bulletin, 184, 114187.

**Exchange Flow and material transport in Chesapeake Bay**

Modified EFDC model to calculate transport timescales for riverine non-conservative materials and surface-produced particulates.

Publication:

Xiong, J., Shen, J. (2022). Vertical transport timescale of surface-produced particulate material in the Chesapeake Bay. Journal of Geophysical Research: Oceans, e2021JC017592.

Xiong, J., Shen, J., Qin, Q. (2021). Exchange flow and material transport along the salinity gradient in a long estuary. Journal of Geophysical Research: Oceans, e2021JC017185.

Xiong, J., Shen, J., Qin, Q., Du, J. (2021). Water exchange and its relationship with external forcings and residence time in Chesapeake Bay. Journal of Marine Systems, 103497.

**Mechanism of high suspended sediment concentration in the southern Yellow Sea, China**

Publication: 

Xiong, J., Wang, X. H., Wang, Y. P., Chen, J., Shi, B., Gao, J., Yang, Y., Yu, Q., Li, M., Yang, L., Gong, X. (2017). Mechanisms of maintaining high suspended sediment concentration over tide-dominated offshore shoals in the Southern Yellow Sea. Estuarine, Coastal and Shelf Science, 191, 221-233.

**wave dynamics**

Publication:

Xiong, J., You, Z., Li, J., Gao, S., Wang, Q., Wang, Y. P. (2020). Variations of wave parameter statistics as influenced by water depth in coastal and shelf areas. Coastal Engineering, 103717.

Xiong, J., Wang, Y. P., Gao, S., Du, J., Yang, Y. (2018). On estimation of coastal wave parameters and wave-induced shear stress. Limnology and Oceanography: Methods, 16(9): 594-606.

