---
layout: spectre
title: Spatial analysis of IMC data using Spectre
permalink: /spectre/spatial/
---

![IMC](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

<p> </p>

Along with flow, spectral, or mass cytometry data, [Spectre](https://immunedynamics.io/spectre/) enables spatial analysis of [Imaging Mass Cytometry (IMC)](https://immunedynamics.io/resources/imc) data. The Hyperion from Fluidigm (an Imaging Mass Cytometer, IMC) consists of a CyTOF (Helios) instrument, with an imaging module attached to the front. Within the imaging module, a pulsed laser scans and ablates the tissue section in incremental 1 um shots, which are then rastered together into an image, consisting of 30-40 metal signals representing different cellular or tissue markers. In order to analyse this imaging data in R, we developed an extension of Spectre, termed '[SpectreMAP](https://immunedynamics.io/spectre/spatial/)', to import, manage, and visualise TIFF files using RStudio. Once cell segmentation has been performed (using our protocols, or those developed by others), the marker expression data for each cell across multiple images can be calculated and incorporated into a single data.table. Clustering, gating, or image-based classification can then label cellular populations. Subsequently, the relationship between cell types and their spatial arrangement and environments can be calculated using our spatial analysis functions. For an overview of the spatial analysis components, please see **this page (coming soon)**.

<p> </p>

# Software installation and demos

1. Installation and demos

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/172228252/SpectreMAP%20wide.png?version=2&modificationDate=1614467478815&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Getting started with spatial analysis using Spectre (& SpectreMAP)</b></p>
        <p>
          Here we provide links and instructions for downloading the relevant software to perform cell segmentation and spatial analysis. We also provide a demo/worked example for analysing IMC data in SpectreMAP specifically. 
        </p>
          <a href="https://wiki.centenary.org.au/x/tphCCw"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

# Image visualisation

We provide links for common software options for image visualisation. These are not required for cell segmentation, but are helpful for exploration of the raw imaging data.

1. MCD viewer
2. HistoCat++

<p> </p>

# Cell Segmentation

One of the key steps in the analysis of IMC data is cell segmentation. Essentially this uses one of a number of methods to create a 'mask' over each of the cells in the image, which allows us to measure all the signal contained within that cell. Once cells have been segmented from an image, we can then perform a number of single-cell analysis approaches. Here we provide software links, demo data, and protocols for performing cell segmentation on IMC data.

1. Basic nuclear expansion segmentation
2. Bodenmiller segmentation pipeline
3. Multi-cut segmentation pipeline
4. Cell type classification with Ilastik
5. Region classification with Ilastik

<p> </p>

# Spatial analysis workflow steps with Spectre

Here we provide workflows using SpectreMAP to facilitate spatial analysis of IMC data, following cell segmentation.

1. Integrated TIFFs and create SpectreMAP object
2. Spatial analysis 
3. Automated plot generation

<p> </p>

# Other workflows

1. Spatial analysis of IMC data in FlowJo
2. TIFF to FCS
3. HistoCat (MatLab/GUI)

# Other software

1. CytoMapper (R)
2. CytoMAP (Matlab)

<p> </p>
