---
layout: spectre
title: Citation
permalink: /spectre/citation/
---

If you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and on the '[about](https://wiki.centenary.org.au/x/az0MCQ)' page.

<br />

## Generic methods section text

Here we have provided some generic text that you can use for your methods section. This should be adjusted to reflect differences in your analysis workflow, with particular attention paid to elements in italics.

Computational analysis of data was performed using the Spectre R package (Ashhurst et al., 2020), with instructions and source code provided at https://github.com/ImmuneDynamics/spectre. Samples were initially prepared in *FlowJo*, and the population of interest was exported as *raw value CSV files*. Arcsinh transformation was performed on the data in R using a *co-factor of 15* to redistribute the data on a linear scale and compress low end values near zero. The dataset was then merged into a single data.table, with keywords denoting the sample, group, and other factors added to each row (cell). *Batch alignment was performed by computing quantile conversions using reference samples recorded with each batch, and then applied to the samples in each batch using CytoNorm (Van Gassen et al., 2019) in Spectre*. The *FlowSOM* algorithm (Van Gassen et al., 2015) was then run on the merged dataset to cluster the data, where every cell is assigned to a specific cluster and metacluster. Subsequently, the data was downsampled and analysed by the dimensionality reduction algorithm *Uniform Manifold Approximation and Projection (UMAP)* (McInnes, Healy, Melville, 2018) for cellular visualisation. 

<br />
