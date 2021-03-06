# cRegulomedb   
## Overview   
The scripts in this repository are used to build and update the database file used with the R pacakge cRegulome. 
cRegulome is R language interface to access pre-caculated expression correlation of regulome (transcription factors & microRNA)
and genes in cancers.  

## Data sources  
The transcription factors correlation data are obtained from [Cistrome Cancer](http://cistrome.org/CistromeCancer/).
This data is based on integrative analysis of public tarnscription factor ChIP-seq data and The Cancer Genome Atlas
[(TCGA)](https://tcga-data.nci.nih.gov) data. The microRNA correlation data are obtained from [miRCancerdb](https://mahshaaban.shinyapps.io/miRCancerdb/) 
database. [miRCancerdb](https://mahshaaban.shinyapps.io/miRCancerdb/) is based on a similar analysis using [(TCGA)](https://tcga-data.nci.nih.gov)
data and [TargetScan](http://www.targetscan.org) annotations.  

## Build/update the database file  
This repository contains two R scripts; `build_tf.R` and `build_mir.R` and a simple `makefile`. By running `make` in
the a UNIX shell, the build scripts load the required libraries and including [`sqlome`](https://github.com/MahShaaban/sqlome) that includes the nessecary funcions to build the database. To do that locally:  

```
git clone https://github.com/MahShaaban/cRegulomedb
cd cRegulomedb
make
```
## Pre-built copy
A pre-built copy of the database file can be obtained from [here](https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/9537385/cRegulome.db.gz).

## More    
+ For more about the cRegulome R package, [here](https://github.com/MahShaaban/cRegulome).  
+ For Citations, [here]().  


