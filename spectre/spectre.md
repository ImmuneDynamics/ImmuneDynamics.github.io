---
layout: spectre-new
title: Spectre Home Page
permalink: /spectre/
---

Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional cytometry data from different batches or experiments. Spectre streamlines the analytical stages of raw data pre-processing, batch alignment, data integration, clustering, dimensionality reduction, visualisation and population labelling, as well as quantitative and statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by data and laboratory scientists. The package was developed by [Thomas Ashhurst](https://tomashhurst.github.io/) (Sydney Cytometry Facility, The University of Sydney), [Felix Marsh-Wakefield](https://scholar.google.com/citations?user=6PaVkisAAAAJ&hl=en) (Discipline of Pathology, The University of Sydney), and [Givanna Putri](https://scholar.google.com/citations?user=S-sNLPIAAAAJ&hl=en) (School of IT, The University of Sydney). For more information on the Spectre, check out the '[about Spectre](https://wiki.centenary.org.au/x/az0MCQ)' page or check out [this talk](https://youtu.be/poEDERGXrQw?t=3151). If you are interested in testing new 'development' functions in Spectre, or adding your own function, see the developers guide. 

![Spectre](https://wiki.centenary.org.au/download/attachments/146080606/sketch-image-1615023265755.png?version=1&modificationDate=1615023277206&api=v2)

**Citation:** if you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and on the 'about' page.

<br />

## Getting started

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

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/159435971/image2020-8-21_9-36-10.png?version=1&modificationDate=1598002570816&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Initial data preparation</b></p>
        <p>Here we provide instructions for initial data preparation, including compensation, cleanup gating, and data export from programs such as FlowJo.</p>
          <a href="https://wiki.centenary.org.au/display/SPECTRE" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />

## Core analysis workflows

---

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Simple discovery workflow
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Batch alignment workflow
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Advanced quantitative and statistical analysis
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-28_12-3-31.png?version=1&modificationDate=1614474211754&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-45-0.png?version=1&modificationDate=1613891282558&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A simple workflow (with worked example) using a single R script to run clustering/dimensionality reduction, make plots, and perform some limited quantitative/statistical analysis. No batch alignment steps included.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A comprehensive and adaptable workflow (with worked example) for the integration and analysis of data from multiple batches.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A workflow to rapidly generate graphs and heatmaps from summary data to perform quantitative and statistical analysis.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/4C8MCQ" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/zORfCQ" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/display/SPECTRE" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />


## Specialised analysis areas

---

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
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Spatial analysis
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
            <img src="https://wiki.centenary.org.au/download/thumbnails/186841491/sketch-image-1613951983362.png?version=1&modificationDate=1614855791266&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide a time-series clustering workflow using ChronoClust.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Analysis workflows for high-dimensional imaging mass cytometry (IMC) data, using Spectre and SpectreMAP, an extension of Spectre, to facilitate spatial analysis.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/Fdb3C" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
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
                      <a href="https://wiki.centenary.org.au/display/SPECTREMAP" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

## Advanced applications

---

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Integrating data derived from different experiments or instruments
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Automated cell classification
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Workflows to manage larger-than-memory datasets
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/157272386/image2021-1-22_18-5-23.png?version=1&modificationDate=1611299123953&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-21_22-15-46.png?version=1&modificationDate=1613906146172&api=v2" width="3000" style="padding-top: 5px; padding-left: 40px; padding-right: 40px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_15-17-53.png?version=1&modificationDate=1613891307741&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Alignment strategies to integrate data from separate experiments or instruments.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Strategies to facilitate automated cell classification.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Strategies for the analysis of very large datasets, that are larger than the memory capacity of the computer being used.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <b><span style="font-size: 16px">IN DEVELOPMENT</span></b>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <b><span style="font-size: 16px">IN DEVELOPMENT</span></b>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                     <b><span style="font-size: 16px">IN DEVELOPMENT</span></b>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

## Tutorials

---

Coming soon...

- Rapidly generate tSNE/UMAP plots from CSV or FCS files
- Convert CSV to FCS files (and vise versa)
- Computational analysis in FlowJo

- Thinking about computational analysis approaches
- Strategic use of clustering and dimensionality reduction
- Batch alignment strategies

- Plotting with Spectre and ggplot2
- Data handling using data.table

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />










## Analysis workflows for specific areas

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:40%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/image2020-8-20_14-46-9.png?version=1&modificationDate=1597937846914&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:60%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Mass (CyTOF), flow, or spectral cytometry analysis with Spectre</b></p>
        <p>Analysis workflows for high-dimensional mass (CyTOF), flow, or spectral cytometry data. Includes data preparation, data transformation (ArcSinh etc), batch alignment, clustering, dimensionality reduction, plotting, and statistical analysis.</p>
          <a href="https://wiki.centenary.org.au/x/k-kiCw"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:40%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/image2021-2-22_10-59-32.png?version=1&modificationDate=1613951972477&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:60%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Analysis tools and functions to assist in the analysis of scRNAseq data</b></p>
        <p>Analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.</p>
          <a href="https://wiki.centenary.org.au/x/l-kiCw"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:40%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/sketch-image-1613951983362.png?version=2&modificationDate=1613952082081&api=v2" width="3000">
      </td>
      <td style="padding-left:.75em;width:60%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Spatial analysis of Imaging Mass Cytometry (IMC) data</b></p>
        <p>Analysis workflows for high-dimensional imaging mass cytometry (IMC) data, using Spectre and SpectreMAP, an extension of Spectre, to facilitate spatial analysis.</p>
          <a href="https://wiki.centenary.org.au/display/SPECTREMAP"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />
<br />
<br />
<br />



<p style="color:grey"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>
