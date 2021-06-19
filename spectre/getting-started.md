---
layout: spectre
title: Getting started
permalink: /spectre/getting-started/
---

You can install Spectre directly using R and RStudio, or install a pre-built R environment containing Spectre using Docker. 

## Option 1: Install Spectre with R and RStudio

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://rstudio.com/wp-content/uploads/2018/10/RStudio-Logo-Flat.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><h2>
          Install R and RStudio
        </h2></p>
        <p>
          Spectre is a software package in 'R'. We recommend interacting with Spectre and the R code via RStudio. Download the latest version of R and R Studio by visiting the links below.
        </p>
        <a href="https://cran.r-project.org/mirrors.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Download R (CRAN)
        </span></b></a>
         | 
        <a href="https://www.rstudio.com/products/rstudio" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Download RStudio
        </span></b></a>
        <br />
         <p>
          Once you have installed R and RStudio, you can check out this
          <a href="https://wiki.centenary.org.au/x/MIBfCQ">tutorial</a>
          to get familiar with using it.
        </p>
        <a href="https://wiki.centenary.org.au/x/MIBfCQ" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            R & RStudio tutorial
        </span></b></a>
        <p> </p>
      </td>
      </tr>
    </tbody>
</table>


<p> </p>


<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://dl3.cbsistatic.com/catalog/2017/12/19/9bbc46dc-1d94-45d0-977a-e4e776e0588d/imgingest-1712473237099407863.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><h2>
          Install XQuartz (for mac users)
        </h2></p>
        <p>
          For mac users only, X11 (including tcltk) requires XQuartz to be installed since it is no longer part of OS X. Always re-install XQuartz when upgrading your macOS to a new major version.
        </p>
        <a href="http://xquartz.macosforge.org/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Install XQuartz
        </span></b></a>
        <p> </p>
      </td>
      </tr>
    </tbody>
</table>


<p> </p>


<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/Spectre%20wide.png?version=1&modificationDate=1614253260985&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><h2>
          Installing and updating Spectre package from Github
        </h2></p>
        <p>
          Once you have installed R and RStudio, the instructions for install and updating Spectre from Github (current default choice) is described below on this page. If you are unfamiliar with using R or RStudio, first check out this
          <a href="https://wiki.centenary.org.au/x/MIBfCQ">
            tutorial
          </a>
          .
        </p>
        <a href="https://wiki.centenary.org.au/x/7-kiCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Install from Github
        </span></b></a>
        <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

Please note: the original functions and workflows for spatial analysis from **SpectreMAP** have now been directly incorporated in **Spectre v0.5.0**.

<br />








## Option 2: Install Spectre using Docker

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/150442594/docker_facebook_share.png?version=1&modificationDate=1580942055355&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><h2>
          Install R, RStudio, and Spectre from Docker
        </h2></p>
        <p>
          Install a 'container' version of Spectre using Docker, that contains a pre-built environment with all the required packages necessary to use Spectre.
        </p>
        <a href="https://wiki.centenary.org.au/x/F4hfCQ" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Install from Docker
        </span></b></a>
        <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

Please note: the original functions and workflows for spatial analysis from **SpectreMAP** have now been directly incorporated in **Spectre v0.5.0**.

<br/>







# Analysis workflows and protocols

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width3035%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spectre protocols for cytometry analysis</b></p>
        <p>
          Here we provide protocols and instructions for using Spectre for the analysis of high-dimensional flow, spectral, or mass (CyTOF) cytometry data. This includes workflows and strategies for performing alignment/integration of data generated in different batches or experiments.
        </p>
          <a href="https://immunedynamics.io/spectre/cytometry/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spatial.png?raw=true" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spatial (IMC) analysis</b></p>
        <p>Here we provide protocols and instructions for using Spectre for the spatial analysis of Imaging Mass Cytometry (IMC) data.</p>
          <a href="https://immunedynamics.github.io/spectre/spatial/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/189556619/image2021-2-22_10-59-32.png?version=1&modificationDate=1615782193059&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Support for scRNAseq analysis</b></p>
        <p>
          Though Spectre was not designed explicitly to work with genomic data, a number of Spectre's processing, analysis, or plotting functions can be helpful in analysing scRNAseq data. Here we provide analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.
        </p>
          <a href="https://wiki.centenary.org.au/x/l-kiCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<br/>





## Other

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_18-50-20.png?version=1&modificationDate=1613893820633&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spectre tutorials</b></p>
        <p>Here we provide tutorials and other worked examples for further education on Spectre and computational analysis more broadly.</p>
          <a href="https://immunedynamics.github.io/spectre/tutorials/"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:30%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/150442594/GitHub-Mark.png?version=1&modificationDate=1580941974093&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:70%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><h2>
          Install a development version of Spectre
        </h2></p>
        <p>
          If you are interested in testing new features, or contributing your own, you can also install the development version of Spectre from Github. We suggested using in conjunction with our <a href="https://wiki.centenary.org.au/x/lMj3C" target="_blank" rel="noopener noreferrer">developers guide</a>.
        </p>
        <a href="https://wiki.centenary.org.au/x/TKNmCg" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">
            Install development version
        </span></b></a>
        <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

<br />
