---
layout: research2
title: Human Cell Atlas
permalink: /research/humancellatlas/
---

### What is the Human Cell Atlas project

The [Human Cell Atlas (HCA)](https://www.humancellatlas.org/) project is international endeavour to create comprehensive reference maps of all cells in the human body. This collection of molecular single-cell maps will provide enormous insight into cellular biology, as well as providing a reference database from which automated cellular classification can be achieved. These efforts are partnered by other atlas-level projects, including the [LifeTime initiative](https://lifetime-initiative.eu/) and the NIH [Human BioMolecular Atlas Program (HubMAP) consortium](https://hubmapconsortium.org/).

### Multi-modal single-cell technologies

Much of the data generated for the various single-cell and inflammatory atlas projects are generated using single-cell RNA sequencing (scRNAseq). In increasing frequency, datasets are being generated by incorporating multi-modal technologies, such as CITE-seq, where transcripts and antibodies on single-cells can be measured simultaneously. The presence of antibody labelling in these atlas datasets allows for direct integration between single-cell atlas datasets and independent high-dimensional cytometry datasets. An example of thise approach is described in [Hao 2020](https://www.biorxiv.org/content/10.1101/2020.10.12.335331v1), where CyTOF and CITE-seq data was integrated together using tools such as [Azimuth](https://azimuth.hubmapconsortium.org/).

### Interfacing with atlas datasets using Spectre

Challenges
- Different challenges and requirements in analysis
- Large cell volumes
- Differences in QC and pre-processing
- Differences in # of features, and implications for integration etc

Our approaches
- Interface with data portals, or download data and do it manually...
- Find common features
- Re-render the resolvable populations in the reference dataset
- Perform alignment
- Perform label transfer

### Further cell atlas resources and guidelines

In addition to direct interactions 

seeking to help define the contribution of high-dimensional cytometry and imaging technologies to the HCA objectives (Czechowska et al. 2018, WS06: ‘Cytometry in the Era of the Human Cell Atlas’).