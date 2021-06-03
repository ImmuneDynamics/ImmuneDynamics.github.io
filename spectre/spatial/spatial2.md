---
layout: spectre
title: Spatial analysis of high-dimensional imaging data using Spectre
permalink: /spectre/spatial2/
---

![IMC](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

[Spectre](https://immunedynamics.io/spectre/) enables the analysis of high-dimensional imaging data, including data generated using Fluidigm's [Hyperion Imaging Mass Cytometer (IMC)](https://immunedynamics.io/resources/imc). Our current workflows support a basic (using CellProfiler) or comprehensive (using Ilastik) cell and region segmentation approach, followed by cellular and spatial analysis using FlowJo or R. 

<p> </p>

<br />





## Overview of cell segmentation and spatial analysis with Spectre

---

Spectre can be used for the analysis of various high-dimensional imaging dataset.

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/Spatial.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:66%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Analysis overview</b></p>
        <p>Here we provide background information on methods of analysing IMC data.
        </p>
          <a href="https://wiki.centenary.org.au/x/_pxCCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<br />






## Initial visualisation, TIFF export, and cell segmentation

---

Below we provide instructions for two key segmentation approaches. The simple nuclear expansion approach is straightforward and involves few moving parts, and the advanced multicut approach is more complex, but extremely versatile, and faciltates regional segmentation as well. In addition to these primary segmentation approaches, we also provide a modified version of the [Bodenmiller lab segmentation approach](https://wiki.centenary.org.au/x/kYBfCQ).

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Image visualisation and TIFF export
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Segmentation option 1: simple nuclear expansion with CellProfiler
        </div>  
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Segmentation option 2: advanced multicut boundary segmentation with Ilastik
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://images.squarespace-cdn.com/content/v1/4f5013cf24ac3afbd1aa0384/1521081849883-SU5OULKJHBQ018D5T8YE/ke17ZwdGBToddI8pDm48kAuB-BVTm5dtGprDXgFPIyUUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYy7Mythp_T-mtop-vrsUOmeInPi9iDjx9w8K4ZfjXt2dru9rxahcePG1TnnIZfTn0BuL3PTOoqn3UWqsetf8ileCjLISwBs8eEdxAxTptZAUg/LN.png?format=750w" width="3000" style="padding-top: 5px; padding-left: 20px; padding-right: 20px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://wiki.centenary.org.au/download/thumbnails/188913604/image2021-2-24_14-38-47.png?version=1&modificationDate=1614305624125&api=v2" width="3000" style="padding-top: 5px; padding-left: 30px; padding-right: 30px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/188913604/image2021-2-24_14-38-20.png?version=1&modificationDate=1614305624416&api=v2" width="3000" style="padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            Here we provide links for common software options for image visualisation. From here, TIFF files can be exported for use in our segmentation approaches.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            This is the simplest form of cellular segmentation. The nuclear signal is identified, and the boundary is expanded outwards by a certain number of pixels. This then becomes the boundary of the cell mask. Although a very simplistic approach, only nuclear signal is required.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            Some IMC images contain extremely dense collections of cells, where cytoplasmic (and sometimes) nuclear signal from one cell is difficult to distinguish from another. In this protocol we describe boundary-based segmentation using the 'multi-cut' workflow in Ilastik.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
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
                      <a href="https://wiki.centenary.org.au/x/GzrDCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/fCnDCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<p> </p>

<br />









## Cellular and spatial analysis

---

Following cell segmentation using one of the above approaches, these workflows facilitate cellular and spatial analysis in R.

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">FCS conversion and analysis in FlowJo
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Simple spatial analysis with Spectre
        </div>  
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Advanced spatial analysis with Spectre (including region masks)
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://flowjowebsiteimages.s3-us-west-2.amazonaws.com/media/Solution%20Logos/flowjo-logo.png" width="3000" style="padding-top: 20px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spatial.png?raw=true" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="" width="3000" style="padding-top: 5px">
      </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            An analysis protocol to facilitate the creation of FCS files from IMC data and subsequent analysis using FlowJo.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            A simple analysis workflow in Spectre, using simple cell masks. 
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
            A more advanced workflow in Spectre, incorporating cell type and region masks for enhanced spatial analysis.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/RHbDCw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <b><span style="font-size: 18px">COMING SOON</span></b>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <b><span style="font-size: 18px">COMING SOON</span></b>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<p> </p>

<br />



















# Other software and protocols

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
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<p> </p>

<br />
