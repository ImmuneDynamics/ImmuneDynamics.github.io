---
layout: spectre
title: Spatial analysis of IMC data using Spectre
permalink: /spectre/spatial/
---

![IMC](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

<p> </p>

Along with flow, spectral, or mass cytometry data, Spectre enables spatial analysis of Imaging Mass Cytometry (IMC) data. The Hyperion from Fluidigm (an Imaging Mass Cytometer, IMC) consists of a CyTOF (Helios) instrument, with an imaging module attached to the front. Within the imaging module, a pulsed laser scans and ablates the tissue section in incremental 1 um shots, which are then rastered together into an image, consisting of 30-40 metal signals representing different cellular or tissue markers. In order to analyse this imaging data in R, we developed an extension of Spectre, termed 'SpectreMAP', to import, manage, and visualise TIFF files using RStudio. Once cell segmentation has been performed (using our protocols, or those developed by others), the marker expression data for each cell across multiple images can be calculated and incorporated into a single data.table. Clustering, gating, or image-based classification can then label cellular populations. Subsequently, the relationship between cell types and their spatial arrangement and environments can be calculated using our spatial analysis functions. For an overview of the spatial analysis components, please see **this page**.

<p> <p/>

# Software installation and demos

1. xxx

<p> <p/>

# Image visualisation

1. MCD viewer
2. HistoCat++

<p> <p/>

# Cell Segmentation

1. Basic nuclear expansion segmentation
2. Bodenmiller segmentation pipeline
3. Multi-cut segmentation pipeline

<p> <p/>

# Spatial analysis workflow steps with Spectre

1. Integrated TIFFs and create SpectreMAP object
2. Spatial analysis 
3. Automated plot generation

<p> <p/>

# Other workflows

1. Spatial analysis of IMC data in FlowJo
2. Cell type classification with Ilastik
3. Region classification with Ilastik

<p> <p/>
