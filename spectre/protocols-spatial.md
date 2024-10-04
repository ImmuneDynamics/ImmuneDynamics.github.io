---
layout: spectre
title: Spectre - Spatial Analysis
permalink: /spectre/spatial/
---

Spectre enables the analysis of high-dimensional imaging data, including data generated using Fluidigm’s Hyperion Imaging Mass Cytometer (IMC). Our current workflows support a basic (using CellProfiler) or comprehensive (using Ilastik) cell and region segmentation approach, followed by cellular and spatial analysis using FlowJo or Spectre (in R). For those gettings started with analysis, first check out our [getting started](https://immunedynamics.github.io/spectre/getting-started/) page for installation instructions and some basic tutorials. 

*Please note: the original functions and workflows from SpectreMAP have now been directly incorporated in Spectre.* 

<br />

## Overview

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/Spatial.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Introduction to cell segmentation and spatial analysis</b></p>
        <p>
          Here we provide background information on methods of analysing IMC data. 
        </p>
         <a href="https://wiki.centenary.org.au/x/_pxCCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
      </td>
      </tr>
    </tbody>
</table>

<br />


## Image visualisation and TIFF export

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://images.squarespace-cdn.com/content/v1/4f5013cf24ac3afbd1aa0384/1521081849883-SU5OULKJHBQ018D5T8YE/ke17ZwdGBToddI8pDm48kAuB-BVTm5dtGprDXgFPIyUUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYy7Mythp_T-mtop-vrsUOmeInPi9iDjx9w8K4ZfjXt2dru9rxahcePG1TnnIZfTn0BuL3PTOoqn3UWqsetf8ileCjLISwBs8eEdxAxTptZAUg/LN.png?format=750w" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Image visualisation and TIFF export</b></p>
        <p>
          Here we provide instructions for initial image visualisation and TIFF export using <a href="https://immunedynamics.io/spectre/spatial/visualisation/">MCD Viewer</a> or <a href="https://immunedynamics.io/spectre/spatial/visualisation/">HistoCat++</a>. From here, TIFF files can be exported for use in our segmentation approaches.
        </p>
         <a href="https://immunedynamics.io/spectre/spatial/visualisation/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
      </td>
      </tr>
    </tbody>
</table>

<br />


## Cell segmentation

Here we provide protocols for performing initial cell segmentation.

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Boundary-based multicut segmentation with Ilastik
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Simple nuclear expansion segmentation with CellProfiler
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Modified Bodenmiller lab segmentation approach
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://avatars.githubusercontent.com/u/895767?s=280&v=4" width="3000" style="padding-top: 5px">
       </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
        <br />
        <br />
          <img src="https://cellprofiler.org/files/files/cellprofiler/files/2017_11_21-cp_logo_black_tm_4.png" width="3000" style="padding-top: 5px">
      </td>
            <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://upload.wikimedia.org/wikipedia/en/c/cd/Anaconda_Logo.png" width="3000" style="padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
             Some IMC images contain extremely dense collections of cells, where cytoplasmic (and sometimes) nuclear signal from one cell is difficult to distinguish from another. In this protocol we describe boundary-based segmentation using the 'multi-cut' workflow in Ilastik. Additional cell type and region masks can be included, which dramatically enhances analysis.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            This is the simplest form of cellular segmentation and analysis. The nuclear signal is identified, and the boundary is expanded outwards by a certain number of pixels. This then becomes the boundary of the cell mask. Although a very simplistic approach, only nuclear signal is required.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            In this approach, the user trains a classifier to identify and predict 'nuclear', 'cytoplasmic', or 'background' pixels. This can be used to create more comprehensive cell masks than can be achieved using simple pixel expansion methods. This is based on the Bodenmiller lab workflow described here. Additional cell type and region masks can be included, which dramatically enhances analysis.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/fCnDCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/GzrDCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/kB-mCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br/>


## Spatial analysis

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Advanced spatial analysis workflow using Spectre (following Ilastik multicut segmentation)
        </div>
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Simple spatial analysis workflow using Spectre (following CellProfiler nuclear expansion segmentation)
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">
          Spatial data analysis using FlowJo
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000" style="padding-top: 5px">
            <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spatial.png?raw=true" width="3000" style="padding-top: 5px">
       </td>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000" style="padding-top: 5px">
            <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/spectre/images/Spatial%20basic.png?raw=true" width="3000" style="padding-top: 5px">
       </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://flowjowebsiteimages.s3-us-west-2.amazonaws.com/media/Solution%20Logos/flowjo-logo.png" width="3000" style="padding-top: 5px">
        <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/spectre/images/Spatial%20FlowJo2.png?raw=true" width="3000" style="padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
           <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            An analysis workflow in R using Spectre that facilitates simultaneous cellular and spatial analysis following boundary-based segmentation with the multicut module of Ilastik..
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            An analysis workflow in R using Spectre that facilitates simultaneous cellular and spatial analysis following nuclear-expansion segmentation in CellProfiler.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            A workflow for analysing IMC data using FlowJo, after initial conversion of TIFF files and masks into FCS files.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/spatial-advanced" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/spatial-simple" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/spatial-flowjo" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>

<br/>

## Other software and protocols

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
          <img src="https://bodenmillergroup.github.io/histocat-web/assets/histocat.png" width="3000" style="padding-top: 5px">
      </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://github.com/BodenmillerGroup/cytomapper/raw/master/vignettes/cytomapper_sticker.png" width="3000" style="padding-top: 5px; padding-left: 50px; padding-right: 50px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <p> </p>
            <p> </p>
            <img src="https://global.discourse-cdn.com/business4/uploads/imagej/optimized/3X/4/d/4d6e06e4a30aef82baf85f6b389d1ec7120a7547_2_690x388.png" width="3000" style="padding-top: 5px">
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
