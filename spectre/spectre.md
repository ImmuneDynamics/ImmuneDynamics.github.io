---
layout: spectre
title: Spectre Home Page
permalink: /spectre/
---

**Overview**: Spectre is an R package and computational toolkit that enables comprehensive end-to-end integration, exploration, and analysis of high-dimensional [cytometry](https://immunedynamics.io/spectre/cytometry/) or [imaging](https://immunedynamics.github.io/spectre/spatial/) data from different batches or experiments. Spectre streamlines the analytical stages of raw data pre-processing, batch alignment/integration, clustering, dimensionality reduction, visualisation, population annotation, and quantitative/statistical analysis; with a simple, clear, and modular design of analysis workflows, that can be utilised by both data and laboratory scientists. 

See our [about](https://immunedynamics.github.io/spectre/about/) page for more information, and check out our [getting started](https://immunedynamics.github.io/spectre/getting-started/), [protocols](https://immunedynamics.github.io/spectre/#protocols), or [tutorial](https://immunedynamics.github.io/spectre/tutorials/) pages to start using Spectre.

![Spectre](https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spectre.png?raw=true)

![IMC](https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/spectre/image2021-2-25_22-32-15.png?raw=true)

<p> </p>

# News

---

**See our [latest version](https://github.com/ImmuneDynamics/Spectre/releases/latest)**

[![AppVeyor build status](https://ci.appveyor.com/api/projects/status/akhvb8wub6d6xhtd?svg=true)](https://ci.appveyor.com/project/tomashhurst/spectre)

To receive updates, you can join our mailing list [here](https://forms.gle/vrg58485Ri5wagRr7).

- 2021-09-03: [v1.0.0 release](https://github.com/ImmuneDynamics/Spectre/releases) including major updates to our [spatial functions and workflows](https://immunedynamics.io/spectre/spatial/).
- 2021-06-04: Spatial [v0.5.0 release](https://github.com/ImmuneDynamics/Spectre/releases) - analysis functions and workflows from SpectreMAP now incorporated directly in Spectre.
- 2021-04-10: Spectre manuscript published online in [Cytometry A](https://doi.org/10.1002/cyto.a.24350)
- 2021-03-30: Updated list of [papers that have referenced Spectre](https://immunedynamics.io/spectre/metrics/) (and/or CAPX and associated scripts).
- 2021-03-08: Spectre [v0.4.0 release](https://github.com/ImmuneDynamics/Spectre/releases) – including significant improvements, as well as the addition of new batch alignment functions.
- 2020-10-23: Spectre pre-print now online: [Ashhurst TM, Marsh-Wakefield F, Putri GH, et al. (2020). bioRxiv](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1).
- 2019-07-31: Spectre Github repository established.
- 2019-05-11: The 'CAPX' workflow (the initial version of Spectre) published as part of a methods chapter of ['Mass Cytometry: Methods and Protocols'](https://link.springer.com/book/10.1007/978-1-4939-9454-0) book: [Ashhurst TM et al. (2019)](https://link.springer.com/protocol/10.1007/978-1-4939-9454-0_12).
- 2018-09-25: [CAPX Github](https://github.com/sydneycytometry/CAPX) established.

<br/>

# Getting started

---

<table class="table gmisc_table">
  <tbody>
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:35%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:middle">
          <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/Spectre%20logo%20wide.png" width="3000">
      </td>
      <td style="padding-left:.75em;width:65%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">
        <p><b>Getting started with R, RStudio, and Spectre</b></p>
        <p>Here we provide instructions for installing R, RStudio, and Spectre, along with introductory tutorials for getting started.</p>
          <a href="https://immunedynamics.github.io/spectre/getting-started/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
          <p> </p>
      </td>
      </tr>
    </tbody>
</table>

<p> </p>

**Citation**: if you use Spectre in your work, please consider citing [Ashhurst TM, Marsh-Wakefield F, Putri GH et al. (2021). Cytometry A. DOI: 10.1002/cyto.a.24350](https://doi.org/10.1002/cyto.a.24350). To continue providing open-source tools such as Spectre, it helps us if we can demonstrate that our efforts are contributing to analysis efforts in the community. Please also consider citing the authors of the individual packages or tools (e.g. [CytoNorm](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.23904), [FlowSOM](https://onlinelibrary.wiley.com/doi/full/10.1002/cyto.a.22625), [tSNE](https://lvdmaaten.github.io/publications/papers/JMLR_2008.pdf), [UMAP](https://arxiv.org/abs/1802.03426), etc) that are critical elements of your analysis work. We have provided some generic text that you can use for your methods section with each protocol and on the '[citation](https://immunedynamics.github.io/spectre/citation)' page.

<p> </p>

<br/>

# Protocols

---

<table class="table gmisc_table">
  <tbody>
<!-- FIRST ROW: TITLE --> 
    <tr style="border-top:1px solid grey">
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Spectre protocols for cytometry analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Spatial (IMC) analysis
        </div>
      </td>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top; background-color:#FAFAFA">
        <div style="text-align:center;font-size:large;font-weight:300;color:#00003f">Support for scRNAseq analysis
        </div>
      </td>
    </tr>
<!-- THIRD ROW: Image --> 
    <tr>
      <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <img src="https://wiki.centenary.org.au/download/attachments/186841491/image2020-8-20_14-46-9.png?version=1&modificationDate=1613891282510&api=v2" width="3000" style="padding-left: 20px; padding-right: 20px; padding-top: 5px">
      </td>
       <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
            <img src="https://github.com/ImmuneDynamics/ImmuneDynamics.github.io/blob/master/images/Spatial.png?raw=true" width="3000" style="padding-top: 5px">
        </td>
        <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #FAFAFA;border-right:1px solid #000;text-align:left; vertical-align:top">
          <p> </p>
            <img src="https://wiki.centenary.org.au/download/attachments/189556619/image2021-2-22_10-59-32.png?version=1&modificationDate=1615782193059&api=v2" width="3000" style="padding-top: 5px">
        </td>
      </tr>
<!-- FOURTH ROW: Description --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide protocols and instructions for using Spectre for the integration and analysis of high-dimensional flow, spectral, or mass (CyTOF) cytometry data. 
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top">Here we provide protocols and instructions for using Spectre for the spatial analysis of Imaging Mass Cytometry (IMC) data.
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #FAFAFA;border-bottom:1px solid #000;border-right:1px solid #000;text-align:left; vertical-align:top"> Here we provide analysis options and tools to support scRNAseq analysis, in conjunction with existing tools such as Seurat and SingleCellExperiment.
          </td>
     </tr>
<!-- FIFTH ROW: Go to page --> 
      <tr>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.io/spectre/cytometry/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
                  </p>
              </div>
          </td>
          <td style="padding-left:.75em;padding-right:.75em;width:33%; border-left:1px solid #000;border-top:1px solid #000;border-bottom:1px solid #000;border-right:1px solid #000;text-align:center; vertical-align:middle">
              <div style="text-align:center;font-size:large;font-weight:700;">
                  <p style="color:#00003f">
                      <a href="https://immunedynamics.github.io/spectre/spatial/" target="_blank" rel="noopener noreferrer"><b><span style="font-size: 18px">GO TO PAGE</span></b></a>
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
      </tr>
    </tbody>
</table>

<br />








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
