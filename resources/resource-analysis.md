---
layout: resource
title: Resources - Computational Analysis
permalink: /resources/analysis
---

![Clusters](https://raw.githubusercontent.com/tomashhurst/tomashhurst.github.io/master/images/Clusters%20wide.png)

**COMPUTATIONAL ANALYSIS**: here we provide resources to facilitate computational analysis of high-dimensional cytometry data, including [Spectre](https://immunedynamics.github.io/spectre/), an R package that enables comprehensive end-to-end integration and analysis of high-dimensional cytometry data from different batches or experiments.

**Webinars and tutorials**:

- Talk on clustering and dimensionality reduction at the ACS 'homeshow': [Youtube](https://www.youtube.com/embed/MSIDmYhqe5g).

<br />

## Resources developed by our group

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>Spectre R package</h2></p>
        <p>
          Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional cytometry data from different batches or experiments. 
          Spectre streamlines the analytical stages of raw data pre-processing, batch alignment, data integration, clustering, dimensionality reduction, visualisation and population labelling, as well as quantitative and statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by data and laboratory scientists. You can find out more from the Spectre home page (below) or from our <a href="https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract">pre-print</a>.
    <p> </p>
       <a href="https://immunedynamics.github.io/spectre" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/189556619/image2021-2-26_11-50-32.png?version=1&modificationDate=1615782192994&api=v2" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>Clustering and dimensionality reduction approaches in FlowJo</h2></p>
        <p>
         Here we provide a protocol for performing clustering and dimensionality reduction using FlowJo, following Spectre's 'Discovery Analysis' workflow.
    <p> </p>
       <a href="https://wiki.centenary.org.au/x/mYGoBw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/CC.jpg" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>ChronoClust</h2></p>
        <p>
          A novel clustering and cluster tracking algorithm specifically designed to cluster and track cellular populations in temporal cytometry data. For each time-point, ChronoClust uses density based clustering algorithms which cluster cells into microclusters (MCs) and thereafter daisy-chained those MCs to form clusters. The evolution of clusters are then tracked by the virtue of their MCs over time.
    <p> </p>
       <a href="https://github.com/ghar1821/chronoclust" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/TrackSOM.png" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>TrackSOM</h2></p>
        <p>
          A temporal clustering and tracking algorithm which fuses ChronoClust’s tracking methodology with the clustering prowess of FlowSOM. In summary, TrackSOM amalgamates data from all time-point into one dataset, and thereafter cluster them using the Self Organising Map (SOM). For each time-point, TrackSOM then isolates the non-empty SOM nodes for that time-point, and perform consensus hierarchical clustering on them. Tracking of the resulting meta-clusters then ensues, by virtue of the SOM nodes.
    <p> </p>
       <a href="https://github.com/ghar1821/TrackSOM" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/Spatial.png" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>Spatial analysis of IMC data using Spectre & SpectreMAP</h2></p>
        <p>
          Along with flow, spectral, or mass cytometry data, Spectre enables spatial analysis of Imaging Mass Cytometry (IMC) data. Here we provide protocols for image visualisation, cell segmentation, and spatial analysis, including with FlowJo.
    <p> </p>
       <a href="https://immunedynamics.github.io/spectre/spatial" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<br />

## Resources developed by others

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://onlinelibrary.wiley.com/cms/asset/481aa823-a644-4fc8-988c-f9d9f9f4e61a/cytoa22625-fig-0001-m.jpg" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>FlowSOM</h2></p>
        <p>
          Using self-organizing maps for visualization and interpretation of cytometry data. Published:
          <a href="https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-020-3469-y">Van Gassen et al. (2015). Cytometry A</a>
    <p> </p>
       <a href="https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.22625" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:25%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
          <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1186%2Fs12859-020-3469-y/MediaObjects/12859_2020_3469_Fig2_HTML.png?as=webp" width="3000" style="padding-top: 30px">
      </td>
      <td style="padding-left:.75em;width:75%; border-left:1px solid #FFFFFF;border-top:1px solid #FFFFFF;border-bottom:1px solid #FFFFFF;border-right:1px solid #FFFFFF;text-align:left; vertical-align:top">
        <p><h2>Brick plots</h2></p>
        <p>
          BrickPlots - a visualisation tool for clustered high dimensional cytometry data. The Brick plot method generates a two-dimensional barcode that displays the phenotype of each cluster in relation to the entire dataset. Brick plots can be used to visualize complex mass cytometry data, both from fundamental research and clinical trials, as well as flow cytometry data. Published:
          <a href="https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-020-3469-y">Norton et al. (2020). BMC Bioinformatics</a>
    <p> </p>
       <a href="https://github.com/NortonS1/BrickPlots" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
        </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

