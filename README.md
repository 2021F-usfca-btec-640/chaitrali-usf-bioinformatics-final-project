# README for SARS-CoV-2 Variant Analysis project

* Chaitrali Deshpande
* PSM Biotechnology First year
* cdeshpande@dons.usfca.edu

## Goals:
Analyze the SARS-CoV-2 patient's Gnome sequence data for Brazil available on NCBI website.

## Project Description
This project aims to analyze the Gnome sequences of SARS-CoV-2 virus infected patients from Brazil collected by NCBI under BioProject PRJNA774631 and released on 10/27/2021.
Through this analysis, I am trying to evaluate the correlation between the SNPs identified in the Gnome and patient geo location or patient sex.

### SRA Bioproject Accession Number: PRJNA774631
URL: https://www-ncbi-nlm-nih-gov.ezproxy.u-pec.fr/Traces/study/?acc=PRJNA774631&o=acc_s%3Aa
Geo loc name country: Brazil
Host Disease: Covid19
SRA Study: SRP343167
Platform: Illumina
Number of sequence data: 66

## Steps Followed:
1. Download the metadata (SraRunTable) for Brazil from the NCBI website.
2. Programmatically retrieve the Gnome sequence data for Run IDs present in the metadata. 
3. Using the BASH pipeline through makefile, process the Gnome sequence data to obtain vcf files for the run. 4. Use R script to stack the vcf files and add SNPs present in the Gnome to the SraRunTable. 
5. Write an Rmarkdown file to analyze the SNP data based on geo location name within Brazil and host sex; discuss and create plots to visualize the findings.
6. Create a presentation to showcase the findings.

## To run the code use makefile
 

### Log
2021-12-15: Created tables listing total samples of host sex, geography and total cases per 100k inhabitants.
2021-12-14: Plotted COVID-19 data against total count of unique SNPs.
2021-12-13: Added Brazil COVID-19 statistics from June 1st, 2021. Also, added tables o
2021-12-12: The Bash Pipeline successfully downloaded the sequence data for runs present in metadata and processed them to create vcf files.
2021-12-12: Metadata file is imported into data/00_SRATable.
2021-12-12: README file updated.
