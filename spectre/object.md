---
layout: spectre
title: Spectre object
permalink: /spectre/object/
---

Notes on the design of the 'Spectre' object.

<pre>
  <code>
    # Comment
    code
  </code>
</pre>

<br />

## Spectre v1

---

Spectre v1 uses a simple table structure to store data, based on the data.table framework. Here cells = rows, and markers/genes = columns (as is the convention for cytometry data). 

For example, this demo dataset consists of 169004 cells, with 9 cellular markers, from 12 samples:

<pre>
  <code>
cell.dat <- Spectre::demo.start
cell.dat
  </code>
</pre>

<pre>
  <code>
                 FileName      NK11        CD3     CD45       Ly6G    CD11b      B220      CD8a       Ly6C       CD4
     1:   CNS_Mock_01.csv   42.3719  40.098700  6885.08  -344.7830 14787.30  -40.2399   83.7175   958.7000  711.0720
     2:   CNS_Mock_01.csv   42.9586 119.014000  1780.29  -429.6650  5665.73   86.6673   34.7219   448.2590  307.2720
     3:   CNS_Mock_01.csv   59.2366 206.238000 10248.30 -1603.8400 19894.30  427.8310  285.8800  1008.8300  707.0940
     4:   CNS_Mock_01.csv  364.9480  -0.233878  3740.04  -815.9800  9509.43  182.4200  333.6050   440.0710  249.7840
     5:   CNS_Mock_01.csv  440.2470  40.035200  9191.38    40.5055  5745.82 -211.6940  149.2200    87.4815  867.5700
    ---                                                                                                             
169000: CNS_WNV_D7_06.csv  910.8890  72.856100 31466.20  -316.5570 28467.80   -7.7972 -271.8040 12023.7000 1103.0500
169001: CNS_WNV_D7_06.csv  -10.2642  64.188700 45188.00  -540.5140 22734.00  202.4110 -936.4920  4188.3300  315.9400
169002: CNS_WNV_D7_06.csv -184.2910  -9.445650 11842.60   -97.9383 17237.00  123.4760 -219.9320  8923.4000 -453.4640
169003: CNS_WNV_D7_06.csv  248.3860 229.986000 32288.20  -681.1630 19255.80 -656.0540 -201.5880 10365.7000   61.6765
169004: CNS_WNV_D7_06.csv  738.9810  95.470300 46185.10 -1004.6000 22957.80 -661.6280   72.3356  9704.4700  -31.8532
  </code>
</pre>



When data processing (e.g. asinh transformation) or analysis (r.g. clustering, dimensionality reduction) is performed, new columns are simply added to the table. 

For example, to asinh transform the cellular columns:

<pre>
  <code>
cols <- names(cell.dat)[c(2:10)]
cell.dat <- do.asinh(cell.dat, cols)
  </code>
</pre>

<pre>
  <code>
                 FileName      NK11        CD3     CD45       Ly6G    CD11b      B220      CD8a       Ly6C       CD4
     1:   CNS_Mock_01.csv   42.3719  40.098700  6885.08  -344.7830 14787.30  -40.2399   83.7175   958.7000  711.0720
     2:   CNS_Mock_01.csv   42.9586 119.014000  1780.29  -429.6650  5665.73   86.6673   34.7219   448.2590  307.2720
     3:   CNS_Mock_01.csv   59.2366 206.238000 10248.30 -1603.8400 19894.30  427.8310  285.8800  1008.8300  707.0940
     4:   CNS_Mock_01.csv  364.9480  -0.233878  3740.04  -815.9800  9509.43  182.4200  333.6050   440.0710  249.7840
     5:   CNS_Mock_01.csv  440.2470  40.035200  9191.38    40.5055  5745.82 -211.6940  149.2200    87.4815  867.5700
    ---                                                                                                             
169000: CNS_WNV_D7_06.csv  910.8890  72.856100 31466.20  -316.5570 28467.80   -7.7972 -271.8040 12023.7000 1103.0500
169001: CNS_WNV_D7_06.csv  -10.2642  64.188700 45188.00  -540.5140 22734.00  202.4110 -936.4920  4188.3300  315.9400
169002: CNS_WNV_D7_06.csv -184.2910  -9.445650 11842.60   -97.9383 17237.00  123.4760 -219.9320  8923.4000 -453.4640
169003: CNS_WNV_D7_06.csv  248.3860 229.986000 32288.20  -681.1630 19255.80 -656.0540 -201.5880 10365.7000   61.6765
169004: CNS_WNV_D7_06.csv  738.9810  95.470300 46185.10 -1004.6000 22957.80 -661.6280   72.3356  9704.4700  -31.8532

         NK11_asinh    CD3_asinh CD45_asinh  Ly6G_asinh CD11b_asinh   B220_asinh  CD8a_asinh Ly6C_asinh   CD4_asinh
     1:  0.04235923  0.040087962   2.627736 -0.33829345    3.388057 -0.040229048  0.08362002  0.8518665  0.66171351
     2:  0.04294540  0.118734817   1.340828 -0.41743573    2.435282  0.086559169  0.03471493  0.4344615  0.30263135
     3:  0.05920201  0.204803270   3.022631 -1.25101677    3.684212  0.415750122  0.28212257  0.8876036  0.65846851
     4:  0.35729716 -0.000233878   2.029655 -0.74509796    2.948184  0.181423123  0.32770787  0.4269784  0.24725691
     5:  0.42713953  0.040024513   2.914359  0.04049443    2.449108 -0.210143906  0.14867171  0.0873703  0.78456678
    ---                                                                                                            
169000:  0.81693878  0.072791800   4.142314 -0.31149515    4.042229 -0.007797121 -0.26856390  3.1817517  0.95239703
169001: -0.01026402  0.064144703   4.504101 -0.51715205    3.817492  0.201053740 -0.83574631  2.1394053  0.31090687
169002: -0.18326344 -0.009445510   3.166628 -0.09778240    3.541046  0.123164374 -0.21819650  2.8849492 -0.43920651
169003:  0.24590035  0.228005328   4.168089 -0.63716643    3.651633 -0.616293228 -0.20024703  3.0339681  0.06163746
169004:  0.68430866  0.095325863   4.525922 -0.88462254    3.827279 -0.620947819  0.07227267  2.9683779 -0.03184782
  </code>
</pre>

Then to add samples annotations, clusters, and dimensionality reduciton coordinates:

<pre>
  <code>
                 FileName      NK11        CD3     CD45       Ly6G    CD11b      B220      CD8a       Ly6C       CD4
     1:   CNS_Mock_01.csv   42.3719  40.098700  6885.08  -344.7830 14787.30  -40.2399   83.7175   958.7000  711.0720
     2:   CNS_Mock_01.csv   42.9586 119.014000  1780.29  -429.6650  5665.73   86.6673   34.7219   448.2590  307.2720
     3:   CNS_Mock_01.csv   59.2366 206.238000 10248.30 -1603.8400 19894.30  427.8310  285.8800  1008.8300  707.0940
     4:   CNS_Mock_01.csv  364.9480  -0.233878  3740.04  -815.9800  9509.43  182.4200  333.6050   440.0710  249.7840
     5:   CNS_Mock_01.csv  440.2470  40.035200  9191.38    40.5055  5745.82 -211.6940  149.2200    87.4815  867.5700
    ---                                                                                                             
169000: CNS_WNV_D7_06.csv  910.8890  72.856100 31466.20  -316.5570 28467.80   -7.7972 -271.8040 12023.7000 1103.0500
169001: CNS_WNV_D7_06.csv  -10.2642  64.188700 45188.00  -540.5140 22734.00  202.4110 -936.4920  4188.3300  315.9400
169002: CNS_WNV_D7_06.csv -184.2910  -9.445650 11842.60   -97.9383 17237.00  123.4760 -219.9320  8923.4000 -453.4640
169003: CNS_WNV_D7_06.csv  248.3860 229.986000 32288.20  -681.1630 19255.80 -656.0540 -201.5880 10365.7000   61.6765
169004: CNS_WNV_D7_06.csv  738.9810  95.470300 46185.10 -1004.6000 22957.80 -661.6280   72.3356  9704.4700  -31.8532

         NK11_asinh    CD3_asinh CD45_asinh  Ly6G_asinh CD11b_asinh   B220_asinh  CD8a_asinh Ly6C_asinh   CD4_asinh
     1:  0.04235923  0.040087962   2.627736 -0.33829345    3.388057 -0.040229048  0.08362002  0.8518665  0.66171351
     2:  0.04294540  0.118734817   1.340828 -0.41743573    2.435282  0.086559169  0.03471493  0.4344615  0.30263135
     3:  0.05920201  0.204803270   3.022631 -1.25101677    3.684212  0.415750122  0.28212257  0.8876036  0.65846851
     4:  0.35729716 -0.000233878   2.029655 -0.74509796    2.948184  0.181423123  0.32770787  0.4269784  0.24725691
     5:  0.42713953  0.040024513   2.914359  0.04049443    2.449108 -0.210143906  0.14867171  0.0873703  0.78456678
    ---                                                                                                            
169000:  0.81693878  0.072791800   4.142314 -0.31149515    4.042229 -0.007797121 -0.26856390  3.1817517  0.95239703
169001: -0.01026402  0.064144703   4.504101 -0.51715205    3.817492  0.201053740 -0.83574631  2.1394053  0.31090687
169002: -0.18326344 -0.009445510   3.166628 -0.09778240    3.541046  0.123164374 -0.21819650  2.8849492 -0.43920651
169003:  0.24590035  0.228005328   4.168089 -0.63716643    3.651633 -0.616293228 -0.20024703  3.0339681  0.06163746
169004:  0.68430866  0.095325863   4.525922 -0.88462254    3.827279 -0.620947819  0.07227267  2.9683779 -0.03184782

            Sample Group Batch FlowSOM_cluster FlowSOM_metacluster        Population     UMAP_X    UMAP_Y
     1: 01_Mock_01  Mock     A              23                   2         Microglia -2.3603757  6.201213
     2: 01_Mock_01  Mock     A              55                   2         Microglia  2.7505242  7.119595
     3: 01_Mock_01  Mock     A              64                   2         Microglia -2.9486033  4.012670
     4: 01_Mock_01  Mock     A              53                   2         Microglia  0.6482904  6.481466
     5: 01_Mock_01  Mock     A             110                   4          NK cells -2.3941295  6.975885
    ---                                                                                                  
169000:  12_WNV_06   WNV     A              72                   3 Infil Macrophages -2.9640724 -5.058265
169001:  12_WNV_06   WNV     A              46                   3 Infil Macrophages -1.2644785 -3.555824
169002:  12_WNV_06   WNV     A             133                   3 Infil Macrophages -2.3592682 -2.429467
169003:  12_WNV_06   WNV     A             133                   3 Infil Macrophages -1.9531062 -4.049705
169004:  12_WNV_06   WNV     A             103                   3 Infil Macrophages -0.7404098 -4.686928
  </code>
</pre>

This simple structure is very easy to interact with and manage for high-dimensional cytometry data. It means that various plotting functions are also easy to apply. For example, to make a dimensionality reduction plot:

<pre>
  <code>
make.colour.plot(cell.dat, 'UMAP_X', 'UMAP_Y', 'FlowSOM_metacluster'
</code>
</pre>

![image](https://user-images.githubusercontent.com/11766139/130011484-d80e9a5b-c958-4002-9f85-66122d9b8d4a.png)

<br />
<br />

## Spectre v2

---

The simple data structure in Spectre v1 is one of the most valued features of our users, as the simplicity makes interaction straightforward. While this works for datasets where the feature columns (i.e. 'markers' etc) are in the 10s-100s. However, when managing single-cell sequencing data, the number of cellular features will reach into the 1000's or 10,000's. Additionally, storing RNA sequencing data as a sparse matrix is important to save on memory consumption, which is not currently possible with data.table. Moreover, multi-omic data will include columns/features of different data types, adding to the complexity. The objects in popular single-cell analysis tools (such as Seurat or the SinglCellExperiment objects) provide more structure, but at the cost of added complexity. 

In Spectre v2, we are introducing the 'Spectre object'. The objective is to prioritise simplicity, staying true to the intent of the simple data.table structure used in v1, but incorporating a low level of organisation to facilitate the management of any type of single-cell data. We attempt to stay true to the simple table-oriented design from Spectre v1. To implement this, we have created a simple list structure, which essentially splits up the table into different groups based on columns.

For a dataset 'dat':, running ```dat``` would return the following:

![image](https://user-images.githubusercontent.com/11766139/129833472-44b6c4f6-d23c-436f-bc3d-a6d8e8199ae4.png)
![image](https://user-images.githubusercontent.com/11766139/129833484-14a8048d-7312-4c9c-b509-07da0d0bbf78.png)
![image](https://user-images.githubusercontent.com/11766139/129833493-e901c3d7-4231-40cb-98cb-6dc3835d7d9b.png)

This is a simple list with three slots: ```meta```, ```data```, and ```analysis```.

```dat@meta```: contains row metadata. E.g. sample names, group names, batch names, etc.

![image](https://user-images.githubusercontent.com/11766139/129833472-44b6c4f6-d23c-436f-bc3d-a6d8e8199ae4.png)

<br />

```dat@data```: is a list containing cellular data. E.g. raw data, transformed/scaled data. This can be any form of single-cell data, including cytometry or single-cell sequencing.

![image](https://user-images.githubusercontent.com/11766139/129833484-14a8048d-7312-4c9c-b509-07da0d0bbf78.png)

<br />

```dat@analysis```: is a list containing any kind of derived analysis. E.g. Clusters, dimensionality reduction coordinates, cluster annotations, etc. In the image below they are all stored in one table, but in the updated version they are stored in a similar maner to the data above (e.g. ```dat@analysis$FlowSOM```, ```dat@analysis$UMAP```)

![image](https://user-images.githubusercontent.com/11766139/129833493-e901c3d7-4231-40cb-98cb-6dc3835d7d9b.png)

<br />

As a result, the functions work in largely the same way, but they can now be directed to a specific dataset (e.g. ```run.umap(cell.dat, 'asinh', cols)``` etc).

<br />
<br />
