---
layout: resource
title: Protocol - antibody titration
permalink: /resources/protocol-titration/
---

**Introduction to antibody titration**

Titrating antibodies for flow cytometry is a useful step in effective and economic panel design. This
allows you to determine what concentration of antibody leads to saturation, which usually requires less
than is recommended by the company. It is important to understand that the correct terminology for
discussing antibody titrations is not "number of antibodies per cell", but rather the concentration of the
antibody. Technically this is best described as antibody mass per volume of buffer (ab ug / buffer uL), but
in reality is more often described as stock antibody volume/buffer volume (ab uL / buffer uL). Because
antibodies are in a massive excess compared to the number of cellular targets, the number of cells can
usually be adjusted about 10-fold with minimal affect on staining, if the antibody is used at saturating
concentration (i.e. if an antibody is saturating, you could in theory stain between 1-10 million cells with
little effect on staining). This also means that the total staining volume can be changed with no affect on
staining quality, as long as the concentration is the same (i.e. for an antibody saturating at 1/100, you
could stain 1 million cells in 50uL (0.5 uL ab), 100uL (1uL ab) or 1mL (10uL ab) and get the same staining
quality).

**Starting details**

The cells should be treated as they would be in a normal experiment (i.e. staining volumes, incubation
times, temperatures, centrifuge speeds and times, use of viability stain, use of Fc-block, use of
fixative). In the protocol below, we have described a procedure that is standard for our laboratory.

Key details for the titration experiment:

- 8-point, 2-fold dilution series in a 96-well plate
- Staining volume: 50uL
- Starting concentration for a dilution series: 1/50
- Volume to be transferred between wells: 75uL

![image](https://user-images.githubusercontent.com/11766139/132123089-92d468c9-42bd-4216-b283-e182c1c9df52.png)

**Prepare antibodies (antibody plate)**

- Mark out 8 wells of a 96-well plate
- Place 122.5 uL of FACS into well #1,and 75uL into wells #2-#8
- Antibody volume to add: add 2.5 uL of fluorophore conjugated antibody to well #1 (containing
122.5 uL FACS). The concentration will be 1/50 vol/vol.

- Using a new tip, pipette 75uL from well #1 into well #2 and mix thoroughly
- Using a new tip, pipette 75uL from well #2 into well #3
- … continue up to well #8
- was Using a new tip, pipette 75uL from well #8 and discard into waste
- At this point you should have 8 wells with 75uL of FACS buffer with various antibody dilutions

**Prepare cells (cell plate)**

- Collect cells of interest (e.g. isolate mouse spleen cells)
- Mark 8 wells of a separate 96-well plate (wells #1-#8)
- Into each well, place cells of interest (typically 1x10^6 for flow, 3x10^6 for CyTOF)
- SPIN: 500g, 5min, 4C and discard supernatant
- Optional Fc block
    - Resuspend cells in 50uL of Fc blocking and UV live/dead mixture (1/100 purified antiCD16/32 and 1/1000 UV live/dead in PBS)
    - INCUBATE: 20min, 4C
- SPIN: 500g, 5min, *C and discard supernatant


**Labelling cells**

- Using a multi-well pipette, transfer 50uL of antibody mixture from wells #1-#8 of the antibody
plate, into wells #1-8 of the cell plate and resuspend cells
- INCUBATE: 30min, 4C
- Top up with 200uL FACS buffer, and SPIN: 500g, 5min, 4C and discard supernatant
- Wash x2 in FACS buffer
    - Resuspend in 250uL FACS buffer
    - SPIN: 500g, 5min, 4C and discard supernatant
- Resuspend in 50uL of 4% PFA or Fixation Buffer
- INCUBATE: 10min, RT, in the dark
- Top up with 200uL FACS buffer
- SPIN: 500g, 5min, 4C and discard supernatant
- Resuspend in 100-200uL FACS buffer
- Proceed to flow cytometer or store overnight

**Performing multiple titrations at once**

In order to perform multiple titrations at once, use the same procedure described above for multiple well
simultaneously. This is easiest when using a multi-well pipette.

**Including useful population identifiers**

The protocol above describes how to perform titration on a heterogeneous population of cells. However,
it is often wise to determine the titration of an antibody on a population of interest. In this case, an
antibody against a useful population identifier can be included in each antibody mixture at a fixed
concentration (e.g. if I wanted to look at Ly6C specifically on neutrophils, I might included a fixed
concentration of Ly6G in my antibody mixtures). It is important to remember that in this situation you will
need single colour compensation controls for the two fluorophores being used.

**Concatenation of files on FlowJo**

- Load the titration files onto FlowJo
- Add a new keyword labelled “dilution” or “dilution factor"
- Enter the relevant dilution value for each file (i.e. 1/100 = 100)
- Select all of the files for the same dilution series, then click Workspace > Concatenate Samples
- Under “create additional parameters”, click “choose” and select “dilution")
- This will create a new FCS file with all of the selected files “concatenated” together
- Load the FCS file in a workspace and change the X-axis to “dilution"
- The saturation point is defined as the lowest concentration of antibody where maximal signal
staining is maintained

![image](https://user-images.githubusercontent.com/11766139/132123162-2dc049e8-de5f-428b-93d2-caf2d50e4452.png)
