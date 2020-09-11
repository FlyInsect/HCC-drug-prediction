# HCC-drug-prediction
This project uses the gene expression profile data in GEO of HCC and the compounds's instances data in CMap, combined with PPI network and pathways information, to screen for compounds that may have therapeutic effects on HCC. 

## Quick Start
* code for fold change and corresponding p-value of gene expression value obtained from GEO profiles see [DEG](https://github.com/FlyInsect/DEG/tree/master/homo).
* code for calculating Therapeutic Score(TS) see [
pathway-and-lincs-data-KS-test](https://github.com/FlyInsect/pathway-and-lincs-data-KS-test/tree/master/caculate%20KS-score).

## Date requirements and description 
1.The `CMap compounds instances data` can be downloaded from [Connectivity CMap O2](https://portals.broadinstitute.org/cmap/#) for row data ".cel files" or download pre-processed data matrix "data matrix".  
 
#### Result data 
2.`HCC gene expression profile data` in GEO can be downloaded from [GSE45436](http://www.ncbi.nlm.nih.gov/geo/). 
And mapped each probe to a gene using the `GPL570` platform obtained from GEO and removed the probes if they did not match any gene. see "gene expression data.xlsx".  

3.`PPI network` used is from the Genome-Scale Integrated Analysis of Networks in Tissues [GIANT](http://giant.princeton.edu/).
The sub-network data see "sub-network data.xlsx".  

4."pathways data.xlsx" : The KEGG pathways enriched from 57 genes in the subnetwork(OGS) and related genes using DAVID online web tool.  

5."score of compound-1168.xlsx" :The calculated Therapeutic Score(TS) of CMap compounds ,which also has records in [CTD](http://ctdbase.org/;jsessionid=B7BA689B9C0C5ED32B21F32734663966).


