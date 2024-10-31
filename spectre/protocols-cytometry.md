---
layout: spectre
title: Spectre - Cytometry Analysis
permalink: /spectre/cytometry/
---

This protocol page contains reproducible workflows for different types of cytometry data analysis using Spectre. For those gettings started with analysis, first check out our [getting started](https://immunedynamics.github.io/spectre/getting-started/) page for installation instructions and some basic tutorials. For more educational content you can check out the [tutorials](https://immunedynamics.io/spectre/cytometry/#tutorials/) at the bottom of the page.


<br />

## Overview

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_15-17-53.png?version=1&modificationDate=1613891307741&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b> Introduction to computational analysis and best practices</b></p>
        <p>
          A brief introduction to the advantages and disadvantages of computational 'discovery' approaches, including clustering and dimensionality reduction. Included are two papers describing best practices and planning tips for high-dimensional analysis.
        </p>
         <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/Ec1vR7Q82Y5AtwIqqDyZGIcB07ApU2JurEyiWGcy0mp-CA?e=ULmBte" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
      </td>
      </tr>
    </tbody>
</table>

<br />

## Core analysis workflows

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <!--<tr style="border-top:1px solid grey">-->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Initial data preparation
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Simple discovery workflow
        </div>
      </td>
            <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Discovery workflow with batch alignment using CytoNorm
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image -->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/157279445/image2019-7-4_11-50-14.png?version=1&modificationDate=1582902798592&api=v2" width="3000" style="padding-top: 5px">
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-28_12-3-31.png?version=1&modificationDate=1614474211754&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            Here we provide instructions for initial data preparation, including compensation, cleanup gating, and data export from programs such as FlowJo. 
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A simple workflow (with worked example) using a single R script (or single FlowJo workspace) to run clustering/dimensionality reduction, make plots, and perform some limited quantitative/statistical analysis. No batch alignment steps included.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A analysis workflow for the alignment and analysis of data from multiple batches, using
            <a href="https://github.com/saeyslab/CytoNorm">CytoNorm</a>
            for batch alignment.
          </td>
     </tr>
<!-- FIFTH ROW: R links -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/ES8T0wBKsapHo_q9mFuxsaoBjioEocJWPfetqLyfPEqmhQ?e=wsfclL" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>             
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/simple-discovery" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING Spectre (in R)</span></b></a>
                  </p>
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/ERDgF-9gkPBEkdZkOEmqFlwBslXIz-gb8uYP5qiglivwrA?e=lkpds4" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING FlowJo</span></b></a>
                  </p>                 
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/cytonorm" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING Spectre (in R)</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>


<br />

## Extensions

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Time-series clustering and analysis with TrackSOM
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Scaling analysis in large cytometry datasets using SuperCellCyto
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Simple automated cell classification
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image -->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/thumbnails/186841491/TS.png?version=1&modificationDate=1613891308205&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/spectre/images/SuperCells.png?raw=true" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_22-15-46.png?version=1&modificationDate=1613906146172&api=v2" width="3000" style="padding-top: 5px; padding-left: 40px; padding-right: 40px">
        </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            Clustering analysis of time-series data using the TrackSOM package. Developed by Givanna Putri and Mark Read.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            SuperCellCyto allows for scalable analysis of very large cytometry datasets. Developed by Givanna Putri and the Phipson Lab, based on the SuperCell R package by David Gfeller lab from the University of Lausanne.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            Strategies to facilitate automated cell classification using a kNN classifier.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/tutorials/time_series/TrackSOM-workflow.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://phipsonlab.github.io/SuperCellCyto/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO SITE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                    <a href="https://immunedynamics.io/spectre/tutorials/label_transfer/Automated-classification.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>


<br />


<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">scRNAseq analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Rapidly generate tSNE or UMAP plots from CSV or FCS files
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Rapid generation of graphs and heatmaps for quantitative, differential, and statistical analysis
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image -->
    <tr>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-22_10-59-32.png?version=1&modificationDate=1614855790882&api=v2" width="3000" style="padding-top: 5px">
        </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/tSNEplots.png?raw=true" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/151793632/image2021-2-28_11-49-51.png?version=1&modificationDate=1614473391780&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to automatically generate tSNE or UMAP plots, after tSNE or UMAP has run in programs such as FlowJo.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we present a quick workflow script to rapidly generate graphs and heatmaps for quantitative, differential, and statistical analysis. Note, this can be used on summary data generated by any program, including FlowJo.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page -->
      <tr>
            <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.github.io/spectre/single-cell/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://github.com/sydneycytometry/tSNEplots" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/ETjEow-Oeq5PgWjEv3V6JKkBSAegcpHzCuVtBrhE6jRnlg?e=dZnN70" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

<!-- 2nd table -->
<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <!--<tr style="border-top:1px solid grey">-->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Converting data.table to SCE and vice versa
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Convert CSV to FCS files (and vise versa)
        </div>
      </td>
      <td></td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/spectre/tutorials/datatable_interoperability/images/sce_dt_conversion.png" width="3000" style="padding-top: 5px; padding-left: 25px; padding-right: 25px">
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <!--<p> </p>-->
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-52-10.png?version=1&modificationDate=1613891307575&api=v2" width="3000" style="padding-top: 5px">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-51-43.png?version=1&modificationDate=1613891307671&api=v2" width="3000" style="padding-top: 5px">
        </td>
      <td></td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
          A tutorial on how to convert data.table to SCE and vice versa.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to rapidly convert FCS files to CSV files (or vise versa).
          </td>
          <td></td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/tutorials/datatable_interoperability/sce_support.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://github.com/sydneycytometry/CSV-to-FCS" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td></td>
      </tr>
    </tbody>
</table>


<br />


## Tutorials

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Which markers should I use for clustering?
        </div>
      </td>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">How many cells can I analyse?
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Arcsinh transformation
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
         <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <p> </p>
            <img src="https://wiki.centenary.org.au/download/attachments/166722331/image2020-6-24_13-59-37.png?version=8&modificationDate=1593009229528&api=v2" width="3000" style="padding-top: 5px">
        </td>
             <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/166722331/image2020-6-24_13-59-15.png?version=1&modificationDate=1593007155183&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/159435971/image2020-8-21_9-36-28.png?version=1&modificationDate=1598002589232&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A brief tutorial on determining which markers to use for clustering and dimensionality reduction.
          </td>
                  <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A brief tutorial on assessing how many cells can be analysed using popular clustering (e.g. FlowSOM) and dimensionality reduction (e.g. tSNE, UMAP) techniques.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A tutorial on transformations for cytometry data, specifically using the arcsinh transformations.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/Eddx596T2gpKkYULpZ9nPQcBqF6rjACRP5nrhgqikiYh0w?e=4Wdmyn" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/EcbiWuZ5SyJKlFLnwUsr66kBzpdd70qcT2Rt9YEL0g3jiA?e=V1xeWf" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/EYxO7lsNh6NNnPhjMYVBdo8BoV0QgXrWhs4V-hLQhTfL3A?e=3gGZwP" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Generating 'summary' data
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Creating heatmaps
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Creating comparison graphs/violing plots
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/151792648/Screen%20Shot%202019-10-24%20at%209.46.16%20pm.png?version=1&modificationDate=1591177008888&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/151793632/image2021-1-13_16-46-33.png?version=1&modificationDate=1610556393370&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/151793632/image2021-1-13_16-42-20.png?version=1&modificationDate=1610556141061&api=v2" width="3000" style="padding-top: 5px; padding-left: 25px; padding-right: 25px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A tutorial on generating 'summary' data from analysed 'cellular' data, to be used for quantitative, differential, and statistical analysis.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A tutorial on the use of expression and z-score/fold-change heatmaps in Spectre.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A tutorial on the generation of comparison graphs/violin plots in Spectre.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/ERtVrQYGRkJEvyuZYopWMRkBDUUdXFkONUVWvUnanxRbrw?e=s3cePI" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/EZv6OxbxSeJNtAwU2n7N7gMBouBB-aCx-CyMyMRyvm1mAQ?e=ADhfA6" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/EXbczEErSqxNrv2YR5dn2XkB-hpdJr5vgOhdbDUhFFkemQ?e=H2eVPj" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

<!-- 1st table -->
<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Make plots with Spectre and ggplot2
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Manipulating and filtering data with data.table
        </div>
      </td>
      <td> </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-10-28_12-38-44.png?version=1&modificationDate=1613891308129&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_18-50-20.png?version=1&modificationDate=1613893820633&api=v2" width="3000" style="padding-top: 5px">
        </td>
      <td> </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
         <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Instructions for creating high-quality coloured tSNE/UMAP plots using Spectre's wrapper for ggplot2.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A tutorial on rapid data manipulation and filtering operations for large datasets using data.table.
          </td>
          <td> </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/ETqKGB1kfK9Jnwi4mWdzSPIB9tJnPNgGE_vQnf87KeHraA?e=ZXuuza" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://unisyd-my.sharepoint.com/:b:/g/personal/thomas_ashhurst_sydney_edu_au/EWxzUbrY24BOh2AOAvNpxCwBw45MmAcAGFaQbeKxlwrgRQ?e=SCwJLy" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td> </td>
    </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<br />
