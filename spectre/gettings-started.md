---
layout: spectre
title: Getting started
permalink: /spectre/getting-started/
---

## R and RStudio

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://www.r-project.org/logo/Rlogo.svg" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>
          Install R and RStudio (& XQuartz for mac users)
        </b></p>
        <p>
          Download the latest version of R by visiting https://cran.r-project.org/mirrors.html and selecting a mirror to download R. Download the latest version of R Studio by visiting https://rstudio.com/ and go to download.
        </p>
          <a href="https://cran.r-project.org/mirrors.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Download R
          </span></b></a>
          <a href="https://rstudio.com/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Download RStudio
          </span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>



<br />

## Spectre

---






<br />

## Other

---





**Overview**: Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional cytometry data from different batches or experiments. Spectre streamlines the analytical stages of raw data pre-processing, batch alignment, data integration, clustering, dimensionality reduction, visualisation and population labelling, as well as quantitative and statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by data and laboratory scientists. The package was developed by [Thomas Ashhurst](https://tomashhurst.github.io/) (the [Sydney Cytometry Core Research Facility](https://sydneycytometry.org.au/), The University of Sydney and Centenary Institute), [Felix Marsh-Wakefield](https://scholar.google.com/citations?user=6PaVkisAAAAJ&hl=en) (the School of Medical Sciences, The University of Sydney), and [Givanna Putri](https://scholar.google.com/citations?user=S-sNLPIAAAAJ&hl=en) (the School of IT, The University of Sydney). 

<p> </p>

![Spectre](https://wiki.centenary.org.au/download/attachments/146080606/sketch-image-1615023265755.png?version=1&modificationDate=1615023277206&api=v2)

<p> </p>

Along with flow, spectral, or mass cytometry data, Spectre enables [spatial analysis](https://immunedynamics.github.io/spectre/spatial/) of Imaging Mass Cytometry (IMC) data. Through our extension package, ‘[SpectreMAP](https://immunedynamics.github.io/spectre/spatial/)’, we can import, manage, and visualise TIFF files using RStudio. Once [cell segmentation](https://immunedynamics.github.io/spectre/spatial/) has been performed (using [our protocols](https://immunedynamics.github.io/spectre/spatial/), or those [developed by others](https://immunedynamics.github.io/spectre/spatial/)), the marker expression data for each cell across multiple images can be calculated and incorporated into a single data.table.

<p> </p>

![Spectre3](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

<p> </p>

**More info**: for more information on Spectre, check out the '[about Spectre](https://wiki.centenary.org.au/x/az0MCQ)' page or [this talk](https://youtu.be/poEDERGXrQw?t=3151). If you are interested in testing new 'development' functions in Spectre, or adding your own function, see the [developers guide](https://wiki.centenary.org.au/x/lMj3C). 

**Citation**: if you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and on the '[about](https://wiki.centenary.org.au/x/az0MCQ)' page.

<p> </p>

# News

---

To receive updates, you can join our mailing list [here](https://forms.gle/vrg58485Ri5wagRr7).

- 2021-03-08: Spectre [v0.4.0 release](https://github.com/ImmuneDynamics/Spectre) – including significant improvements, as well as the addition of new batch alignment functions.
- 2020-10-23: Spectre pre-print now online: [Ashhurst TM, Marsh-Wakefield F, Putri GH, et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1).
- 2019-07-31: Spectre Github repository established.
- 2019-05-11: The 'CAPX' workflow (precursor to Spectre) published as part of a methods chapter of 'Mass Cytometry: Methods and Protocols': Ashhurst TM et al. (2019). Methods Mol Biol. 1989:159-192. doi: 10.1007/978-1-4939-9454-0_12.

<p> </p>

# Getting started

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/Spectre%20wide.png?version=1&modificationDate=1614253260985&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Getting started with R, RStudio, and Spectre</b></p>
        <p>Here we provide instructions for installing R, RStudio, and Spectre, along with introductory tutorials for getting started.</p>
          <a href="https://wiki.centenary.org.au/pages/viewpage.action?pageId=150442594" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

# Protocols - cytometry

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spectre protocols for cytometry analysis</b></p>
        <p>Here we provide protocols and instructions for using Spectre for the analysis of cytometry data.</p>
          <a href="https://immunedynamics.github.io/spectre/protocols/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

# Protocols - scRNAseq

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/189556619/image2021-2-22_10-59-32.png?version=1&modificationDate=1615782193059&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spectre protocols for scRNAseq analysis</b></p>
        <p>Here we provide protocols and instructions for using Spectre for the analysis of scRNAseq and CITEseq/Ab-seq data.</p>
          <a href="https://immunedynamics.github.io/spectre/protocols/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>


# Protocols - spatial analysis

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spatial.png?raw=true" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spatial (IMC) analysis</b></p>
        <p>Here we provide protocols and instructions for using Spectre for the spatial analysis of Imaging Mass Cytometry (IMC) data.</p>
          <a href="https://immunedynamics.github.io/spectre/spatial/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

# Tutorials

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_18-50-20.png?version=1&modificationDate=1613893820633&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spectre tutorials</b></p>
        <p>Here we provide tutorials and other worked examples for further education on Spectre and computational analysis more broadly.</p>
          <a href="https://immunedynamics.github.io/spectre/tutorials/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>