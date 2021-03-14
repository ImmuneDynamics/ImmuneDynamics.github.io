---
layout: spectre
title: Spectre - spatial analysis of IMC data
permalink: /spectre/spatial/
---

Along with cytometry data, Spectre can enables the spatial analysis of Imaging Mass Cytometry (IMC) data. This is aided by our extension package 'SpectreMAP', that facilitates the import and management of TIFF files. 

The Hyperion (imaging mass cytometer, IMC) consists of a CyTOF (Helios) instrument, with an imaging module attached to the front. Within the imaging module, a pulsed laser scans and ablates the tissue section in incremental 1 um shots. With each laser shot, vaporised material is carried into the mass cytometer, and the metal ions are analysed by time-of-flight mass spectrometry. SpectreMAP was developed by Thomas Ashhurst (Sydney Cytometry Core Research Facility, The University of Sydney).

**The analysis workflow involves three key steps:**

1. Cell segmentation using one of our approaches using Ilastik and/or CellProfiler.

2. Integrating tiff files, masks, and cellular data into SpectreMAP's spatial data object in R.

3. Performing cellular (clustering, dimensionality reduction) and spatial (region, distance, neighbour) analysis of the IMC dataset.
