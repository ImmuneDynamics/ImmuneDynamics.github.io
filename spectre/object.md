---
layout: spectre
title: Spectre objecct
permalink: /spectre/object/
---

## About the Spectre object

---

Spectre v1 uses a simple table structure (rows = cells vs columns = features) for analysis, using the data.table framework (which extends the functionality of the classic data.frame to allos for extremely efficient processing of large datasets). When data transformation (e.g. asinh transformation) or analysis (r.g. clustering, dimensionality reduction) is performed, new columns are simply added to the table. This simple structure is very easy to interact with and manage for high-dimensional cytometry data, where the number of feature columns (i.e. 'markers' etc) are in the 10s-100s. However, when managing single-cell sequencing/multi-omic data, the number of cellular features will reach into the 1000's or 10,000's. Objects in popular single-cell analysis tools (such as Seurat or the SinglCellExperiment objects) provide more structure, but at the cost of added complexity. 

In Spectre v2, we are introducing the 'Spectre object', which is meant to prioritise simplicity. Fundamentally, we attempt to stay true to the simple table-oriented design from Spectre v1, but allows for larger numbers of cellular features. To implement this, we have created a simple list structure, which essentially splits up the table into different groups based on columns.

For a dataset 'dat':

`dat@meta`: contains row metadata. E.g. sample names, group names, batch names, etc.
`dat@data`: is a list containing cellular data. E.g. raw data, transformed/scaled data. This can be any form of single-cell data, including cytometry or single-cell sequencing.
`dat@analysis`: is a list containing any kind of derived analysis. E.g. Clusters, dimensionality reduction coordinates, cluster annotations, etc.

...

<br />
<br />