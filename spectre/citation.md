---
layout: spectre
title: Citation
permalink: /spectre/citation/
---

## Referencing 'Spectre'

If you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2021). Cytometry A. DOI: 10.1002/cyto.a.24350](https://doi.org/10.1002/cyto.a.24350). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and below.

**To see a list of publications that have used Spectre, please check out our [metrics](https://immunedynamics.io/spectre/metrics/) page.**

<br />

---

## Generic methods section text

_Here we have provided some generic text that you can use as an exmaple to write your own methods section. This should be updated to reflect the details used in your experiments (especially those italicised below). Please note this is an example/template only, we recommend writing your own version of the methods section to avoid duplicating text that might appear in other publications._

Computational analysis of data was performed using the Spectre R package ([Ashhurst et al., 2021](https://doi.org/10.1002/cyto.a.24350)), with instructions and source code provided at [https://github.com/ImmuneDynamics/spectre](https://github.com/ImmuneDynamics/spectre). Samples were initially prepared in *FlowJo*, and the population of interest was exported as *raw value CSV files*. Arcsinh transformation was performed on the data in R using a *co-factor of 15* to redistribute the data on a linear scale and compress low end values near zero. The dataset was then merged into a single data.table, with keywords denoting the sample, group, and other factors added to each row (cell). *Batch alignment was performed by computing quantile conversions using reference samples recorded with each batch, and then applied to the samples in each batch using CytoNorm ([Van Gassen et al., 2019](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.23904)) in Spectre*. The *FlowSOM* algorithm ([Van Gassen et al., 2015](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.22625)) was then run on the merged dataset to cluster the data, where every cell is assigned to a specific cluster and metacluster. Subsequently, the data was downsampled and analysed by the dimensionality reduction algorithm *Uniform Manifold Approximation and Projection (UMAP)* ([McInnes, Healy, Melville, 2018](https://arxiv.org/abs/1802.03426)) for cellular visualisation. 

**References**

- [Integration, exploration, and analysis of high-dimensional single-cell cytometry data using Spectre. 2021. TM Ashhurst, F Marsh-Wakefield, GH Putri, et al., Cytometry A. DOI: 10.1002/cyto.a.24350](https://doi.org/10.1002/cyto.a.24350)
- [S Van Gassen, B Gaudilliere, MS Angst, Y Saeys, N Aghaeepour. (2020). CytoNorm: a normalization algorithm for cytometry data. Cytometry Part A 97 (3), 268-278](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.23904)
- [S Van Gassen et al. (2015). FlowSOM: Using self‐organizing maps for visualization and interpretation of cytometry data. Cytometry Part A 87 (7), 636-645](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.22625)
- [L McInnes, J Healy, J Melville. (2018). UMAP: Uniform Manifold Approximation and Projection for Dimension Reduction. arXiv: 1802.03426.](https://arxiv.org/abs/1802.03426)


<br />
