---
layout: spectre
title: Spatial analysis of high-dimensional imaging data using Spectre
permalink: /spectre/spatial/
---

Spectre enables the analysis of high-dimensional imaging data, including data generated using Fluidigm’s Hyperion Imaging Mass Cytometer (IMC). Our current workflows support a basic (using CellProfiler) or comprehensive (using Ilastik) cell and region segmentation approach, followed by cellular and spatial analysis using FlowJo or Spectre (in R). *Please note: the original functions and workflows from SpectreMAP have now been directly incorporated in Spectre.*

<br/>




## Getting started

---

Here we provide some helpful resources and protocols for getting started. 

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Overview of cell segmentation and spatial analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Image visualisation and TIFF export
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Installing Spectre (R)
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/Spatial.png" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://images.squarespace-cdn.com/content/v1/4f5013cf24ac3afbd1aa0384/1521081849883-SU5OULKJHBQ018D5T8YE/ke17ZwdGBToddI8pDm48kAuB-BVTm5dtGprDXgFPIyUUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYy7Mythp_T-mtop-vrsUOmeInPi9iDjx9w8K4ZfjXt2dru9rxahcePG1TnnIZfTn0BuL3PTOoqn3UWqsetf8ileCjLISwBs8eEdxAxTptZAUg/LN.png?format=750w" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://rstudio.com/wp-content/uploads/2018/10/RStudio-Logo-Flat.png" width="3000" style="padding-top: 5px; padding-right: 20px">
          <img src="https://wiki.centenary.org.au/download/attachments/146080606/Spectre%20wide.png?version=1&modificationDate=1614253260985&api=v2" width="3000">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide background information on methods of analysing IMC data.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide instructions for initial image visualisation and TIFF export using <a href="https://immunedynamics.io/spectre/spatial/visualisation/">MCD Viewer</a> or <a href="https://immunedynamics.io/spectre/spatial/visualisation/">HistoCat++</a>. From here, TIFF files can be exported for use in our segmentation approaches.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide instructions for installing R, RStudio, and Spectre, along with introductory tutorials for getting started.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/_pxCCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/spatial/visualisation/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.github.io/spectre/getting-started/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br/>
<br/>






## Approach 1. Simple cell segmentation and analysis with CellProfiler and Spectre

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
          <img src="https://cellprofiler.org/files/files/cellprofiler/files/2017_11_21-cp_logo_black_tm_4.png" width="3000">
        <p> </p>
        <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p>
          This is the simplest form of cellular segmentation and analysis. The nuclear signal is identified, and the boundary is expanded outwards by a certain number of pixels. This then becomes the boundary of the cell mask. Although a very simplistic approach, only nuclear signal is required. Following cell segmentation, the data can be analysed in R using Spectre, or in FlowJo. 
        </p>
        <p>
          <b><span style="font-size: 16px">1. Segmentation: <a href="https://wiki.centenary.org.au/x/GzrDCw" target="_blank" rel="noopener noreferrer">CellProfiler</a></span></b>
        </p>
        <p>
          <b><span style="font-size: 16px">2. Analysis: 
            <a href="https://immunedynamics.io/spectre/spatial-simple" target="_blank" rel="noopener noreferrer">Simple spatial in Spectre (R)</a>
            or
            <a href="https://immunedynamics.io/spectre/spatial-flowjo" target="_blank" rel="noopener noreferrer">in FlowJo</a>
          </span></b>
        </p>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />
<br />










## Approach 2. Advanced cell segmentation and analysis with Ilastik and Spectre

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
        <p> </p>
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Segmentation/Multicut.png?raw=true" width="3000">
          <p> </p>
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000">
        <p> </p>
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p>
          Some IMC images contain extremely dense collections of cells, where cytoplasmic (and sometimes) nuclear signal from one cell is difficult to distinguish from another. In this protocol we describe boundary-based segmentation using the 'multi-cut' workflow in Ilastik. Additional cell type and region masks can be included, which dramatically enhances analysis. Following cell segmentation, the data can be analysed in R using Spectre, or in FlowJo.
        </p>
        <p>
          <b><span style="font-size: 16px">1. Segmentation: <a href="https://wiki.centenary.org.au/x/fCnDCw" target="_blank" rel="noopener noreferrer">Ilastik multicut</a></span></b>
        </p>
        <p>
            <b><span style="font-size: 16px">2. Analysis: 
            <a href="https://immunedynamics.io/spectre/spatial-advanced" target="_blank" rel="noopener noreferrer">Advanced spatial in Spectre (R)</a>
            or
            <a href="https://immunedynamics.io/spectre/spatial-flowjo" target="_blank" rel="noopener noreferrer">in FlowJo</a>
              </span></b>
        </p>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />
<br />













## Other software and protocols

---

Here we provide links to other analysis software and protocols that are useful in the analysis of high-dimensional imaging data.

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">HistoCat (GUI, Matlab)
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">CytoMapper (R)
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">CytoMAP (GUI, Matlab)
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <p> </p>
          <p> </p>
          <img src="https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-21_21-41-21.png?version=1&modificationDate=1613904081230&api=v2" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://github.com/BodenmillerGroup/cytomapper/raw/master/inst/imgs/cytomapper_sticker.png" width="3000" style="padding-top: 5px; padding-left: 50px; padding-right: 50px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <p> </p>
            <p> </p>
            <img src="https://aws1.discourse-cdn.com/business4/uploads/imagej/optimized/3X/4/d/4d6e06e4a30aef82baf85f6b389d1ec7120a7547_2_690x388.png" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">HistoCat software from the Bodenmiller/Shapiro labs.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">CytoMapper software from the Bodenmiller lab.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">CytoMAP software from the Gerner lab.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://github.com/BodenmillerGroup/histoCAT" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">LINK</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://bioconductor.org/packages/release/bioc/html/cytomapper.html" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">LINK</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://gitlab.com/gernerlab/cytomap/-/wikis/home" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">LINK</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br />

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Segmentation/Modified%20bodenmiller.png?raw=true" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Modified Bodenmiller segmentation protocol with Ilastik</b></p>
        <p>
          In this approach, the user trains a classifier to identify and predict 'nuclear', 'cytoplasmic', or 'background' pixels. This can be used to create more comprehensive cell masks than can be achieved using simple pixel expansion methods. This is based on the Bodenmiller lab workflow described here. Additional cell type and region masks can be included, which dramatically enhances analysis.
        </p>
          <a href="https://wiki.centenary.org.au/x/kB-mCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>


<br />
