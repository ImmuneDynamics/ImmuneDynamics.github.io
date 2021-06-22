---
layout: research2
title: Time-series clustering analysis for mapping dynamic immune responses
permalink: /research/time-series/
---

### Immune responeses over time

The immune response to disease is inherently complex, dynamic, and specific. 
While it is mostly effective, the success of an immune response varies not only between diseases, but also between individuals. 
Designing effective intervention in disease requires an in-depth understanding of how the immune response responds to disease over time.
To understand this, time-course experiments are often performed, extracting diseased samples from several time-points, characterising individual cells using cytometry or single-cell methods, and thereafter analysing them to map out the specific times at which cells differentiate or functionally change.
The fundamental challenge to analysing such temporal data is not only the identification of the cellular populations in the dataset, but also the tracking of their phenotypic and functional changes over time.

![TS](https://wiki.centenary.org.au/download/attachments/150459925/image2020-10-7_18-19-39.png?version=1&modificationDate=1602094779678&api=v2)

Whilst there exists clustering approaches such as FlowSOM and Phenograph which identify cellular populations in non-temporal cytometry data, few attempts have been made to develop methodologies which simultaneously cluster cells and track their changes over time. 
To address this, we developed [ChronoClust](https://www.sciencedirect.com/science/article/abs/pii/S0950705119300796) and [TrackSOM](https://github.com/ghar1821/TrackSOM).

<br />

---

### TrackSOM

<div class='row'>
    <div class="image">
        <a href="#">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/TrackSOM.png" alt="icon" width="300" align="left" style="padding-left: 0px; padding-right: 10px; padding-top: 5px; padding-bottom: 10px">
        </a>
    </div>
</div>


**TrackSOM** ([paper](https://www.biorxiv.org/content/10.1101/2021.06.08.447468v1), [Github](https://github.com/ghar1821/TrackSOM)).

[TrackSOM worked example](https://wiki.centenary.org.au/display/SPECTRE/TrackSOM+worked+example)

Building on ChronoClust’s success, we sought to determine whether its tracking methodology could be used to enhance an existing algorithm.
Following our [previous clustering algorithm benchmarking study](https://academic.oup.com/bioinformatics/advance-article-abstract/doi/10.1093/bioinformatics/btab038/6122691) which found FlowSOM clustering algorithm to be extremely effective in clustering benchmark single time-point cytometry data, we developed **TrackSOM** ([paper](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7), [Github](https://github.com/ghar1821/TrackSOM)), a temporal clustering and tracking algorithm which fuses ChronoClust's tracking methodology with the clustering prowess of FlowSOM. 
In summary, TrackSOM amalgamates data from all time-point into one dataset, and thereafter cluster them using the Self Organising Map (SOM).
For each time-point, TrackSOM then isolates the non-empty SOM nodes for that time-point, and perform consensus hierarchical clustering on them.
Tracking of the resulting meta-clusters then ensues, by virtue of the SOM nodes. 

<p> </p>

TrackSOM offers 2 different tracking operations, namely allowing or disallowing merging of meta-cluster, and 3 different clustering operations, Autonomous Adaptive where the number of meta-clusters per time-point is automatically inferred based on the meta-clusters' variance (akin to FlowSOM's elbow criterion), Prescribed Invariant and Variant where the number of meta-clusters in each time-point are either fixed to a number or varied based on user's specification respectively.
We used TrackSOM to study the immune profile of [SARS-CoV-2/COVID-19](https://immunedynamics.github.io/research/disease) patients, and found TrackSOM successfully identified the dynamic activation (CD38 and HLA-DR) of both innate and adaptive cells and their subsequent decline.
Furthermore, we also compared TrackSOM's performance against that of ChronoClust's on the aforementioned WNV-BM dataset, and found TrackSOM to be comparable, if not better than ChronoClust.

---

### ChronoClust

<div class='row'>
    <div class="image">
        <a href="#">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/research/CC.jpg" alt="icon" width="300" align="left" style="padding-left: 0px; padding-right: 10px; padding-top: 5px; padding-bottom: 10px">
        </a>
    </div>
</div>

<!--border: 5px solid #555"-->

**ChronoClust** ([paper](https://www.sciencedirect.com/science/article/abs/pii/S0950705119300796), [Github](https://github.com/ghar1821/chronoclust)) is a novel clustering and cluster tracking algorithm specifically designed to cluster and track cellular populations in temporal cytometry data. 
For each time-point, ChronoClust uses density based clustering algorithms which cluster cells into microclusters (MCs) and thereafter daisy-chained those MCs to form clusters.
The evolution of clusters are then tracked by the virtue of their MCs over time. 
We demonstrated ChronoClust's prowess by analysing a temporal cytometry data elucidating the immune response of West Nile Virus (WNV) infected mice in the bone marrow (WNV-BM).
ChronoClust was able to not only automatically reproduce the clusters and relationships previously determined manually by an expert, but was also able to uncover the temporal changes in cellular populations abundances consistent with existing biological studies.

<br />

---
