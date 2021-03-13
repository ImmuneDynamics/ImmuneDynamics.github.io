---
layout: page
title: Research
permalink: /research/
---

---

- Not a lab -- so our collective interest cover a range of areas in immunology, infectious disease, single-cell and cytometry technologies, computational biology, and data science.
- Our members are interested in XXXXXXX XXXXXX XXXXXXXX

Key areas for ID:

Development
- Cytometry Technologies
- Computational and spatial analysis Tools

Application
- COVID-19
- Viral encephalitis
- Immunology

---

Following a seed funding grant from the [Marie Bashir Institute for Infectious Diseases and Biosecurity](https://www.sydney.edu.au/marie-bashir-institute/), we established the ‘[Immune Dynamics team](https://immunedynamics.io/about)’, a collaboration combining expertise in immunology, high-dimensional single-cell technologies, computational biology, and data science; drawing from the [Sydney Cytometry Core Research Facility](https://sydneycytometry.org.au/), the [Discipline of Pathology](https://www.sydney.edu.au/medicine-health/schools/school-of-medical-sciences/discipline-of-pathology.html), and the [School of Computer Science](https://www.sydney.edu.au/engineering/schools/school-of-computer-science.html), at the [University of Sydney](https://www.sydney.edu.au/). Our team focuses on the development of novel computational analysis tools to address challenges in modern single-cell sciences, and the application of these tools in the study of immunology and infectious diseases, such as [COVID-19](https://immunedynamics.io/research).

We have developed a number of computational analysis approaches, including [Spectre](immunedynamics.io/spectre), an R package that enables comprehensive end-to-end integration and analysis of high-dimensional cytometry data from different batches or experiments ([Ashhurst\*,  Marsh-Wakefield\*, Putri\* et al. bioRxiv. 2020](https://www.biorxiv.org/content/10.1101/2020.10.22.349563v1.abstract)). To facilitate the analysis of time-series data, we have also developed a number of time-series clustering algorithms, including [ChronoClust](https://github.com/ghar1821/Chronoclust) ([Putri et al. 2019](https://www.sciencedirect.com/science/article/pii/S0950705119300796)) and [TrackSOM](https://github.com/ghar1821/TrackSOM), which we recently applied to the study of [COVID-19](https://immunedynamics.io/research) ([Koutsakos et al. 2021](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7)). Most recently, we have adapted the Spectre package to facilitate spatial analysis of IMC data ([SpectreMAP Github](https://github.com/ImmuneDynamics/SpectreMAP)). 

Our ongoing work is focused on the development of better data integration approaches and spatial analysis tools. You can read more about our work on the [research](https://immunedynamics.io/research) page.

![Comp](https://wiki.centenary.org.au/download/attachments/146080606/Screen%20Shot%202020-10-22%20at%2012.25.13%20pm.png?version=1&modificationDate=1603369521998&api=v2)

<br />

## Application to disease ##

---

![COVID](https://raw.githubusercontent.com/tomashhurst/tomashhurst.github.io/master/images/COVID%20image%20wide%202.png)

We apply our high-dimensional technologies and analysis approaches to study inflammation and infectious disease. A particular focus has been the study of *immunopathology*, where the immune response to infection may be a significant driver of disease. 

**SARS-CoV-2 and COVID-19**

The severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2) pandemic has caused >101 million infections and 2.18 million deaths worldwide (as of January 28, 2021). Infection with SARS-CoV-2 results in a spectrum of clinical presentations, called coronavirus disease 2019 (COVID-19), ranging from asymptomatic to fatal disease. Through a collaboration with the [Doherty Institute](https://www.doherty.edu.au/) and the [University of Melbourne](https://www.unimelb.edu.au/), we comprehensively profiled the immune response to [SARS-CoV-2](https://www.who.int/emergencies/diseases/novel-coronavirus-2019) in a cohort of [COVID-19](https://www.who.int/emergencies/diseases/novel-coronavirus-2019) patients. Our work demonstrated that patients with severe disease exhibited an excessive and hyper-activated immune response ([Koutsakos et al. 2021](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7)). To study the kinetics of this immune response, we also developed and applied a novel time-series analysis approach called [TrackSOM](https://github.com/ghar1821/TrackSOM). 

- This study has been featured on [Doherty Instite News](https://www.doherty.edu.au/news-events/news/mapping-an-effective-immune-response-to-covid-19), [Medical Xpress](https://medicalxpress.com/news/2021-02-effective-immune-response-covid-.html), the [Herald Sun](https://www.heraldsun.com.au/coronavirus/melbourne-experts-uncover-why-covid-affects-people-differently/news-story/ed5ffb9604c1b4db776503562e494f71), and [Ticker](https://twitter.com/tickerNEWSau/status/1359991653243572224?s=20).
- Our [webinar](https://www.fluidigm.com/articles/presentation---mapping-dynamic-immunity-across-time-space-and-disease-state-using-high%E2%80%90dimensional-cytometry-technologies-and-analytics) from 2020 (Mapping Immunity Across Time, Space and Disease State) is featured on the Fluidigim ‘[COVID-19 resources](https://www.fluidigm.com/singlearticles/covid-19-resources)’ page.
- Our mass cytometry protocols have been cited in a number of COVID-19 studies, including [Rodriguez et al. 2020](https://doi.org/10.1016/j.xcrm.2020.100078) and [Koutsakos et al. 2021](https://doi.org/10.1016/j.xcrm.2021.100208).
- Panel design and analysis protocols that may be helpful in COVID-19 research can be found on the [resources](https://tomashhurst.github.io/resources) page.

<br />
