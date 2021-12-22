---
layout: spectre
title: About Spectre
permalink: /spectre/about/
---

## Overview

Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional [cytometry](https://immunedynamics.io/spectre/cytometry/) or [imaging](https://immunedynamics.github.io/spectre/spatial/) data from different batches or experiments. Spectre streamlines the analytical stages of raw data pre-processing, batch alignment/integration, clustering, dimensionality reduction, visualisation, population annotation, and quantitative/statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by data and laboratory scientists. The Spectre package was developed by [Thomas Ashhurst](https://immunedynamics.github.io/thomas-ashhurst/) (the [Sydney Cytometry Core Research Facility](https://sydneycytometry.org.au/), The University of Sydney and Centenary Institute), [Felix Marsh-Wakefield](https://immunedynamics.github.io/felix-marsh-wakefield/) (the School of Medical Sciences, The University of Sydney), and [Givanna Putri](https://immunedynamics.github.io/givanna-putri/) (the School of IT, The University of Sydney); with support from Alanna Spiteri, Dr. Diana shinko, Dr. Mark Read, Dr. Adrian Smith, and Prof. Nicholas King.


![Spectre](https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spectre.png?raw=true)

![IMC](https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/spectre/image2021-2-25_22-32-15.png?raw=true)


[Spectre](https://immunedynamics.github.io/spectre) ([Ashhurst et al, 2021](https://doi.org/10.1002/cyto.a.24350)) or '[CAPX](https://github.com/sydneycytometry/CAPX)', the initial version of Spectre ([Ashhurst et al 2019](https://link.springer.com/protocol/10.1007/978-1-4939-9454-0_12)), and associated scripts have been used in a variety of studies, both with our team and independently, including the study of 
[COVID-19](https://www.sciencedirect.com/science/article/pii/S2666379121000197), 
[vaccine](https://www.nature.com/articles/s41385-021-00379-6) responses, 
[NK cell](https://journals.plos.org/plospathogens/article?id=10.1371/journal.ppat.1006999) biology, 
[multiple myeloma](https://ashpublications.org/bloodadvances/article/4/19/4593/463891/Inverse-relationship-between-oligoclonal-expanded), 
[pediatric burns](https://www.frontiersin.org/articles/10.3389/fimmu.2020.01481/full), 
[multiple sclerosis](https://onlinelibrary.wiley.com/doi/full/10.1002/cti2.1133), 
[bone marrow](https://www.frontiersin.org/articles/10.3389/fimmu.2018.01672/full) transplantation, and 
[cerebral malaria](https://www.nature.com/articles/s42003-018-0216-2), 
among others; in prestigious journals such as [Cell](https://doi.org/10.1016/j.cell.2018.08.013) and [Nature Immunology](https://www.researchgate.net/publication/343838774_The_NK_cell_granule_protein_NKG7_regulates_cytotoxic_granule_exocytosis_and_inflammation). It is also a featured analysis package for the [Human Cell Atlas](https://data.humancellatlas.org/analyze/methods/spectre) project. 

***See a full list of publications citing Spectre [here](https://immunedynamics.io/spectre/metrics/)***

<br />

---

## Getting started

See our [about](https://immunedynamics.github.io/spectre/about/) page for more information, and check out our [protocols](https://immunedynamics.github.io/spectre/#protocols) or [tutorial](https://immunedynamics.github.io/spectre/tutorials/) pages to get started. For users unfamiliar with using R, we also provide [workflow instructions](https://immunedynamics.github.io/spectre/#protocols) for replicating many of our analysis approaches in programs such as [FlowJo](https://immunedynamics.github.io/spectre/#protocols). Along with [flow](https://immunedynamics.io/resources/flow), [spectral](https://immunedynamics.io/resources/flow), or [mass cytometry (CyTOF)](https://immunedynamics.io/resources/mass) data, [Spectre](https://immunedynamics.io/spectre/) enables adaptable [cell segmentation](https://immunedynamics.github.io/spectre/spatial/) and [spatial analysis](https://immunedynamics.github.io/spectre/spatial/) of high-dimensional imaging data, such as [Imaging Mass Cytometry (IMC)](https://immunedynamics.io/resources/imc). 

<br />

---

## Background

As the size and complexity of high-dimensional cytometry data continues to expand, comprehensive analysis tools that can scale to large datasets are required. In our early mass cytometry work, the analysis of high-dimensional datasets using manual methods became prohibitive, requiring the use of computational analysis approaches, such as clustering and dimensionality reduction. However, the analysis tools available at the time were not well suited to the analysis of large cytometry datasets, consistings of tens to hundreds of millions of single cells. Furthermore, popular clustering and dimensionality reduction tools alone are insufficient for scalable or reproducible integration of data across batches, experiments, or different cytometry/single-cell technologies. To address these limitations, we initially developed the ‘Cytometry Analysis Pipeline for large and compleX datasets’ ([CAPX](https://github.com/sydneycytometry/CAPX), the initial version of Spectre), an analysis workflow using the R programming language ([Ashhurst et al. 2019](https://link.springer.com/protocol/10.1007/978-1-4939-9454-0_12)), and derivative stand-alone scripts (e.g. '[tSNEplots](https://github.com/sydneycytometry/tSNEplots)'). Following a seed funding grant from the [Marie Bashir Institute for Infectious Diseases and Biosecurity](https://www.sydney.edu.au/marie-bashir-institute/), we established the ‘[Immune Dynamics](https://immunedynamics.io/team)’ team, a collaborative multi-disciplinary group with a focus on the development of novel computational analysis tools to address challenges in high-dimensional analysis, with a particular focus on the analysis of large datasets, and the incorporation of data integration strategies. We solidified the functionality of the [CAPX](https://github.com/sydneycytometry/CAPX) workflow into a package and re-named it '[Spectre](https://immunedynamics.io/spectre/)'. This was initially released as a pre-print in bioRxiv ([Ashhurst\*, Marsh-Wakefield\*, Putri\* et al. bioRxiv. 2020](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract)) and then published in Cytometry A ([Ashhurst\*, Marsh-Wakefield\*, Putri\* et al. Cytometry A. 2020](https://doi.org/10.1002/cyto.a.24350)).

<!--<span class="__dimensions_badge_embed__" data-id="pub.1132092846" data-hide-zero-citations="true" data-legend="always" data-style="small_circle"></span><script async src="https://badge.dimensions.ai/badge.js" charset="utf-8"></script>
<p> </p>-->

<!--<div style="margin-left: 30px"><a href="https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract">Ashhurst*, Marsh-Wakefield*, Putri* et al. bioRxiv. 2020</a></div>
<p> </p>
<script type="text/javascript" src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script><div data-badge-details="right" data-badge-type="donut" data-altmetric-id="92965811" data-hide-no-mentions="true" class="altmetric-embed" style="margin-left: 30px"></div>
<p> </p>-->

<!--<blockquote class="twitter-tweet tw-align-center"><p lang="en" dir="ltr">Thrilled to announce our preprint is out on bioRxiv: <a href="https://t.co/YebSZu94Yq">https://t.co/YebSZu94Yq</a>. Here we present Spectre, an R package that enables comprehensive end-to-end integration and analysis of high-dimensional cytometry data from different batches or experiments. <a href="https://t.co/l1crJst3lO">https://t.co/l1crJst3lO</a> <a href="https://t.co/hcs2rZd8Lk">https://t.co/hcs2rZd8Lk</a> <a href="https://t.co/IX4sa9K9Jf">pic.twitter.com/IX4sa9K9Jf</a></p>&mdash; Dr Thomas Ashhurst (@TomAsh_1) <a href="https://twitter.com/TomAsh_1/status/1320551790199275520?ref_src=twsrc%5Etfw">October 26, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>-->

<br />

---

## What is Spectre

Spectre is an R package designed to facilitate data analysis workflows that simplify and streamline data manipulation and annotation, population identification (clustering, classification), and dimensionality reduction (t-SNE, UMAP) etc in high-dimensional cytometry data. Strategic implementation of batch-alignment, data-integration, and cell-type classification tools allow for the integrated analysis of multiple experiments, as well as a reproducible system for rapid and repeated cell type identification in large datasets. Critically, the fundamental data structures used within Spectre, along with the implementation of classifiers allow for the scalable analysis of very large high-dimensional datasets. In addition to high-dimensional cytometry datasets, we’ve also developed functions to allow for spatial analysis of high-dimensional imaging datasets, such as those generated by Imaging Mass Cytometry. The simple, clear, and modular design of analysis workflows allow for these tools to be used by informaticians and laboratory scientists alike. 

Along with the various R packages used within Spectre, some key packages such as the cytofkit and Seurat R packages provided inspiration for elements of the package design. [Our team](https://immunedynamics.io/team) develops other computational approaches, including tools for the analysis of time-series data (e.g. [ChronoClust](https://github.com/ghar1821/Chronoclust), [Putri et al 2019](https://www.sciencedirect.com/science/article/pii/S0950705119300796); and [TrackSOM](https://github.com/ghar1821/TrackSOM), [Koutsakos et al 2020](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7)) or spatial data (e.g. [SpectreMAP](https://immunedynamics.io/spectre/spatial/)). As our tools reach a stable level of development, we incorporate these into Spectre, so they may form part of a cohesive workflow.

![Spectre2](https://raw.githubusercontent.com/tomashhurst/tomashhurst.github.io/master/images/Clusters%20wide.png)

Along with flow, spectral, or mass cytometry data, Spectre enables [spatial analysis](https://immunedynamics.github.io/spectre/spatial/) of Imaging Mass Cytometry (IMC) data. Through our extension package, ‘[SpectreMAP](https://immunedynamics.github.io/spectre/spatial/)’, we can import, manage, and visualise TIFF files using RStudio. Once [cell segmentation](https://immunedynamics.github.io/spectre/spatial/) has been performed (using [our protocols](https://immunedynamics.github.io/spectre/spatial/), or those [developed by others](https://immunedynamics.github.io/spectre/spatial/)), the marker expression data for each cell across multiple images can be calculated and incorporated into a single data.table.

![Spectre3](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

In the following presentation, we describe the integration, exploration, and analysis of high-dimensional single-cell cytometry data using Spectre in detail, as part of the [Oz Single Cell seminar series](https://youtu.be/poEDERGXrQw?t=3151) 2020.

<p align="center"><iframe width="560" height="315" src="https://www.youtube.com/embed/poEDERGXrQw?start=3151" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

<br />

---

## Spectre built on data.table

Many existing computational tools store data in a custom format, such as the flowFrame or SingleCellExperiment object, that provide excellent field-specific structuring of single-cell data. In Spectre, data management and operations are performed using the data.table format, an extension of R’s base data.frame, provided by the data.table package. This table-like structure organises cells (rows) against cellular features or metadata (columns). This simple data.table structure allows for the high-speed processing, manipulation (subsetting, filtering, etc.), and plotting of large datasets, as well as fast reading/writing of large CSV files.

Rather than storing analysis outputs (clusters, dimensionality reduction values, annotations etc) in separate areas of a custom data format, Spectre simply adds new columns to the existing data.table. The simplicity of this data structure facilitates extremely fast and simple filtering/subsetting by data.table, as every cell (row) contains all of the information relevant for that cell: such as cellular expression, samples/groups, clusters/populations, and dimensionality reduction coordinates.

<br />

---

## Clustering and dimensionality reduction strategies for large datasets

Whilst clustering tools such as FlowSOM scale well to large datasets, dimensionality reduction approaches such as t-SNE and UMAP do not; as they incur lengthy computing time, excessive memory usage, and significant crowding effects that inhibit their utility. Whilst some improvements to runtime (flt-SNE) and plot crowding (opt-SNE) have been made, scalability and plot crowding limitations persist. As dimensionality reduction tools are primarily used to visualise cellular data and clustering results, we plot a subset of the clustered data, which addresses scalability and retains legibility. By using proportional subsampling from each sample, the relative number of cells from each cluster in each sample can be preserved in a smaller dataset, allowing for interpretable analysis via DR. Putative cellular populations amongst the clusters can then be identified, and annotated in both the subsampled DR dataset, as well as the whole clustered dataset. The whole annotated dataset can subsequently be used in downstream quantification and statistical analysis.

<br />
