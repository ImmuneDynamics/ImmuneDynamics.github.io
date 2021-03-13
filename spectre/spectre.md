---
layout: spectre-new
title: Spectre Home Page
permalink: /spectre/
---

Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional cytometry data from different batches or experiments. Spectre streamlines the analytical stages of raw data pre-processing, batch alignment, data integration, clustering, dimensionality reduction, visualisation and population labelling, as well as quantitative and statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by data and laboratory scientists. The package was developed by [Thomas Ashhurst](https://tomashhurst.github.io/) (Sydney Cytometry Facility, The University of Sydney), [Felix Marsh-Wakefield](https://scholar.google.com/citations?user=6PaVkisAAAAJ&hl=en) (Discipline of Pathology, The University of Sydney), and [Givanna Putri](https://scholar.google.com/citations?user=S-sNLPIAAAAJ&hl=en) (School of IT, The University of Sydney). 

![Spectre](https://wiki.centenary.org.au/download/attachments/146080606/sketch-image-1615023265755.png?version=1&modificationDate=1615023277206&api=v2)

For more information on Spectre, check out the '[about Spectre](https://wiki.centenary.org.au/x/az0MCQ)' page or [this talk](https://youtu.be/poEDERGXrQw?t=3151). If you are interested in testing new 'development' functions in Spectre, or adding your own function, see the developers guide. 

**Citation:** if you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and on the 'about' page.

<br />

## News

---

To receive updates, you can join our mailing list [here](https://forms.gle/vrg58485Ri5wagRr7).

- 2021-03-08: Spectre [v0.4.0 release](https://github.com/ImmuneDynamics/Spectre) – including significant improvements, as well as the addition of new batch alignment functions.
- 2020-10-23: Spectre pre-print now online: [Ashhurst TM, Marsh-Wakefield F, Putri GH, et al. (2020). bioRxiv. 2020.10.22.349563](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1).
- 2019-07-31: Spectre Github repository established.
- 2019-05-11: The 'CAPX' workflow (precursor to Spectre) published as part of a methods chapter of 'Mass Cytometry: Methods and Protocols': Ashhurst TM et al. (2019). Methods Mol Biol. 1989:159-192. doi: 10.1007/978-1-4939-9454-0_12.

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
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

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
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">A comprehensive and adaptable workflow (with worked example) for the alignment and analysis of data from multiple batches.
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
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

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
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<br />

## Advanced applications

---

These are approaches that are in use within our team, but are still under active development. These are described in our preprint ([Ashhurst\*, Marsh-Wakefield\*, Putri\*, et al. 2020. bioRxiv](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1)). If you are interested in using any of these approaches, please [get in touch](mailto:thomas.ashhurst@sydney.edu.au) with us.

<p> </p>

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
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<br />

## Tutorials

---


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
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Computational analysis in FlowJo
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/thumbnails/186841491/image2021-2-21_18-49-43.png?version=1&modificationDate=1613894655972&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-52-10.png?version=1&modificationDate=1613891307575&api=v2" width="3000" style="padding-top: 5px">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-21_12-51-43.png?version=1&modificationDate=1613891307671&api=v2" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2021-2-26_11-50-14.png?version=1&modificationDate=1614300742629&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to automatically generate tSNE or UMAP plots, after tSNE or UMAP has run in programs such as FlowJo.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">An R script to rapidly convert FCS files to CSV files (or vise versa).
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">FlowJo has incorporated a number of clustering, dimensionality reduction, and batch alignment tools. This allows for fairly easy use by those familiar with FlowJo. Here we provide protocols for performing Spectre's discovery analysis workflows using FlowJo.
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
                      <a href="https://wiki.centenary.org.au/x/mYGoBw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<br />

Coming soon...

- Choosing a co-factor for arcsinh transformation
- Thinking about computational analysis approaches
- Strategic use of clustering and dimensionality reduction
- Batch alignment strategies
- Plotting with Spectre and ggplot2
- Data handling using data.table
