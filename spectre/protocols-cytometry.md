---
layout: spectre
title: Spectre Protocols - Cytometry
permalink: /spectre/cytometry/
---

This protocol page contains reproducible workflows for different types of analysis using Spectre. For those gettings started with analysis, you can also check out these two commentary papers where we provide considerations for new and experienced users in the design and analysis of high-dimensional experiments: [Marsh-Wakefield et al 2021 (ICB)](https://onlinelibrary.wiley.com/doi/10.1111/imcb.12456), [Liechti et al 2021 (Nature Immunology)](https://www.nature.com/articles/s41590-021-01006-z). For more educational content you can check out the [tutorials](https://immunedynamics.io/spectre/tutorials/) page.

<br />

## Data preparation

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/159435971/image2020-8-21_9-36-10.png?version=1&modificationDate=1598002570816&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Initial data preparation</b></p>
        <p>Here we provide instructions for initial data preparation, including compensation, cleanup gating, and data export from programs such as <a href="https://www.flowjo.com/">FlowJo</a>. For cell isolation and staining protocols for flow, spectral, or mass (CyTOF) cytometry, please see our <a href="https://immunedynamics.githubio/resources">resources</a> page.   
        </p>
          <a href="https://wiki.centenary.org.au/x/1eRfCQ" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />

## Core analysis workflows

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Simple discovery workflow
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Discovery workflow with batch alignment using CytoNorm
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image -->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-28_12-3-31.png?version=1&modificationDate=1614474211754&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A simple workflow (with worked example) using a single R script (or single FlowJo workspace) to run clustering/dimensionality reduction, make plots, and perform some limited quantitative/statistical analysis. No batch alignment steps included.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:50%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A analysis workflow for the alignment and analysis of data from multiple batches, using
            <a href="https://github.com/saeyslab/CytoNorm">CytoNorm</a>
            for batch alignment. If working with very large batch effects, have a look at our
            <a href="https://immunedynamics.github.io/spectre/cytometry/#advanced-applications">data integration</a>
            workflows.
          </td>
     </tr>
<!-- FIFTH ROW: R links -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/simple-discovery" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING Spectre (in R)</span></b></a>
                  </p>
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/mYGoBw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING FlowJo</span></b></a>
                  </p>                 
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/zGCdCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">USING Spectre (in R)</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>


<br />

## Quick analysis scripts

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Rapidly generate tSNE or UMAP plots from CSV or FCS files
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Convert CSV to FCS files (and vise versa)
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
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/tSNEplots.png?raw=true" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <!--<p> </p>-->
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-52-10.png?version=1&modificationDate=1613891307575&api=v2" width="3000" style="padding-top: 5px">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-51-43.png?version=1&modificationDate=1613891307671&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/151793632/image2021-2-28_11-49-51.png?version=1&modificationDate=1614473391780&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to automatically generate tSNE or UMAP plots, after tSNE or UMAP has run in programs such as FlowJo.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to rapidly convert FCS files to CSV files (or vise versa).
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we present a quick workflow script to rapidly generate graphs and heatmaps for quantitative, differential, and statistical analysis. Note, this can be used on summary data generated by any program, including FlowJo.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page -->
      <tr>
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
                      <a href="https://github.com/sydneycytometry/CSV-to-FCS" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/VzedCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>


<br />

## Specialised analysis areas

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE -->
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Time-series analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">scRNAseq analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Automated cell classification
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image -->
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/thumbnails/186841491/TS.png?version=1&modificationDate=1613891308205&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-22_10-59-32.png?version=1&modificationDate=1614855790882&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_22-15-46.png?version=1&modificationDate=1613906146172&api=v2" width="3000" style="padding-top: 5px; padding-left: 40px; padding-right: 40px">
        </td>
      </tr>
<!-- FOURTH ROW: Description -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide a time-series clustering workflow using TrackSOM.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Strategies to facilitate automated cell classification.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page -->
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/research/time-series_workflow/TrackSOM-workflow.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/l-kiCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                    <a href="https://immunedynamics.io/spectre/Automated-classification.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>


<br />
