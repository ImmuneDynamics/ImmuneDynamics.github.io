---
layout: spectre
title: Spatial analysis of IMC data using Spectre
permalink: /spectre/spatial2/
---

![IMC](https://wiki.centenary.org.au/download/attachments/172228252/image2021-2-25_22-32-15.png?version=1&modificationDate=1614252735692&api=v2)

**Please note: These spatial workflows are under active development, and have not yet been published or peer reviewed (unless stated otherwise). As such, these are not ready for widespread use, and should be considered as in a 'beta' test phase. However, they are in use for analysis within our team.** 
If you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2021). Cytometry A. DOI: 10.1002/cyto.a.24350](https://doi.org/10.1002/cyto.a.24350). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. CytoNorm, FlowSOM, tSNE, UMAP, etc) that are critical elements of your analysis work. 

<p> </p>

---

<br />


## Overview of cell segmentation and spatial analysis with Spectre

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
                      <a href="https://wiki.centenary.org.au/x/gDaICw" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/_h_rCg" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://wiki.centenary.org.au/x/tv5DCg" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
      </tr>
    </tbody>
</table>
<p style="color:#d3d3d3; text-align:right"><i>Code for the table structure adapted from https://satijalab.org/seurat</i></p>

<p> </p>

<br />

