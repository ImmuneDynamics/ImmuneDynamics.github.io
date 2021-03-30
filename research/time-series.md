---
layout: research2
title: Time-series clustering analysis for mapping dynamic immune responses
permalink: /research/time-series/
---

### Immune responeses over time

Immune response is inherently complex, dynamic, and specific. 
It protects us from diseases brought about by pathogens by deploying a wide range of nuanced responses which specifically target them. 
While it is mostly effective, the success rate of an immune response vary not only between diseases but also between individuals. 
An immune response may be successful in a person, but not another.
In the event it is not successful, manual effective health-promoting interventions are crucial to prevent fatalities. 
Designing an effective interventions requires an in-depth understanding on how the immune response develop in a disease over time.
To understand this, biologists perform time-course experiments, extracting diseased samples from several time-points, characterising individual cells using cytometry, and thereafter analysing them to map out the specific times at which cells differentiate or functionally change.
The fundamental challenge to analysing such temporal cytometry data is not only the identification of the cellular populations in the dataset, but also the tracking of their phenotypic and functional changes over time.
Whilst there exists clustering approaches such as FlowSOM and Phenograph which identifies cellular populations in non-temporal cytometry data, little attempts have been made to develop methodologies which simultaneously cluster cells and track their changes over time. 
To address this, we developed [ChronoClust](https://www.sciencedirect.com/science/article/abs/pii/S0950705119300796) and [TrackSOM](https://github.com/ghar1821/TrackSOM).

<br />

### ChronoClust

<div class='row'>
    <div class="image">
        <a href="#">
            <img src="https://wiki.centenary.org.au/download/attachments/186841491/TS.png?version=1&modificationDate=1613891308205&api=v2" alt="icon" width="300" align="left" style="padding-left: 0px; padding-right: 10px; padding-top: 5px; padding-bottom: 10px">
        </a>
    </div>
</div>

ChronoClust ([paper](https://www.sciencedirect.com/science/article/abs/pii/S0950705119300796), [Github](https://github.com/ghar1821/chronoclust)) is a novel clustering and cluster tracking algorithm specifically designed to cluster and track cellular populations in temporal cytometry data. 
For each time-point, ChronoClust uses density based clustering algorithms which cluster cells into microclusters (MCs) and thereafter daisy-chained those MCs to form clusters.
The evolution of clusters are then tracked by the virtue of their MCs over time. 
We demonstrated ChronoClust's prowess by analysing a temporal cytometry data elucidating the immune response of West Nile Virus (WNV) infected mice in the bone marrow (WNV-BM).
ChronoClust was able to not only automatically reproduce the clusters and relationships previously determined manually by an expert, but was also able to uncover the temporal changes in cellular populations abundances consistent with existing biological studies.

<br />

### TrackSOM

<div class='row'>
    <div class="image">
        <a href="#">
            <img src="https://raw.githubusercontent.com/ImmuneDynamics/ImmuneDynamics.github.io/master/images/TrackSOM.png" alt="icon" width="300" align="left" style="padding-left: 0px; padding-right: 10px; padding-top: 5px; padding-bottom: 10px">
        </a>
    </div>
</div>

Building on ChronoClust’s success, we were curious as to whether its tracking methodology could be used to enhance an existing algorithm.
Following our [previous clustering algorithm benchmarking study](https://academic.oup.com/bioinformatics/advance-article-abstract/doi/10.1093/bioinformatics/btab038/6122691) which found FlowSOM clustering algorithm to be extremely effective in clustering benchmark single time-point cytometry data, we developed TrackSOM ([paper](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(21)00019-7), [Github](https://github.com/ghar1821/TrackSOM)), a temporal clustering and tracking algorithm which fuses ChronoClust's tracking methodology with the clustering prowess of FlowSOM. 
In summary, TrackSOM amalgamates data from all time-point into one dataset, and thereafter cluster them using the Self Organising Map (SOM).
For each time-point, TrackSOM then isolates the non-empty SOM nodes for that time-point, and perform consensus hierarchical clustering on them.
Tracking of the resulting meta-clusters then ensues, by virtue of the SOM nodes. 

<p> </p>

TrackSOM offers 2 different tracking operations, namely allowing or disallowing merging of meta-cluster, and 3 different clustering operations, Autonomous Adaptive where the number of meta-clusters per time-point is automatically inferred based on the meta-clusters' variance (akin to FlowSOM's elbow criterion), Prescribed Invariant and Variant where the number of meta-clusters in each time-point are either fixed to a number or varied based on user's specification respectively.
We used TrackSOM to study the immune profile of [SARS-CoV-2/COVID-19](https://immunedynamics.io/research/disease) patients, and found TrackSOM successfully identified the dynamic activation (CD38 and HLA-DR) of both innate and adaptive cells and their subsequent decline.
Furthermore, we also compared TrackSOM's performance against that of ChronoClust's on the aforementioned WNV-BM dataset, and found TrackSOM to be comparable, if not better than ChronoClust.

Stay tuned for the publication describing the TrackSOM algorithm! 
