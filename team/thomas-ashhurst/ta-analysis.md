---
layout: ta
title: Thomas Ashhurst - Computational Analysis
permalink: /thomas-ashhurst/analysis/
---

<!--![Comp](https://wiki.centenary.org.au/download/attachments/146080606/Screen%20Shot%202020-10-22%20at%2012.25.13%20pm.png?version=1&modificationDate=1603369521998&api=v2)-->

![Research](https://raw.githubusercontent.com/tomashhurst/tomashhurst.github.io/master/images/Research.png)

In our early mass cytometry work, the analysis of high-dimensional datasets using manual methods became prohibitive, requiring the use of **computational analysis** approaches. However, the analysis tools available at the time were not well suited to the analysis of large cytometry datasets, consistings of millions of single cells. To address these limitations, I developed the 'Cytometry Analysis Pipeline for large and compleX datasets' (CAPX), an analysis workflow using the R programming language ([Ashhurst et al. 2019](https://link.springer.com/protocol/10.1007/978-1-4939-9454-0_12)). 

Following a seed funding grant from the [Marie Bashir Institute for Infectious Diseases and Biosecurity](https://www.sydney.edu.au/marie-bashir-institute/) ("Mapping dynamic immunity: next-generation computational approaches to track the evolution of immune responses in West Nile virus and Zika virus encephalitis"), we established the ‘[Immune Dynamics](https://github.com/ImmuneDynamics)’ team, a collaborative group with a focus on the development of novel computational analysis tools to address challenges in high-dimensional analysis. My team and I have developed a number of computational analysis approaches, including [SPECTRE](https://wiki.centenary.org.au/display/SPECTRE), an R package that enables comprehensive end-to-end integration and analysis of high-dimensional cytometry data from different batches or experiments ([Ashhurst\*,  Marsh-Wakefield\*, Putri\* et al. bioRxiv. 2020](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract)). Spectre allows for... ... ... This work lead to the participation of members of the team  (Dr. Thomas Ashhurst, Dr. Felix Marsh-Wakefield, and Givanna Putri) as speakers in the ACS [High-Dimensional Cytometry Analysis](https://www.immunology.org.au/files/Newsletter_pdfs/ASI017_Dec_2020.pdf#page=35) in 2020. 

To facilitate the **analysis of time-series data**, we have also developed a number of time-series clustering algorithms, including [ChronoClust](https://github.com/ghar1821/Chronoclust) ([Putri et al. 2019](https://www.sciencedirect.com/science/article/pii/S0950705119300796)) and [TrackSOM](https://github.com/ghar1821/TrackSOM), which we recently applied to the study of [COVID-19](https://tomashhurst.github.io/research/#application-to-disease) ([Koutsakos et al. 2021](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7)). We have also developed novel multi-perspective methods for the evaluation of clustering algorithms ([Putri et al. 2021](https://doi.org/10.1093/bioinformatics/btab038)). 

Most recently, we have adapted the Spectre package to facilitate **spatial analysis** of IMC data ([SpectreMAP Github](https://github.com/ImmuneDynamics/SpectreMAP)).

Our currenty efforts... our ongoing work is focused on the development of better data integration approaches and spatial analysis tools.

<br />
