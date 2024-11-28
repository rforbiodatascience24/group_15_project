# 22160: R for Bio Data Science
# Exploration and differential gene-expression analysis of TCGA - LUAD samples - Group 15

Authors:

José Dinis Coelho da Silva Ferreira (s212484)

Maria Gabriela Frascella (s231331)

Paula Gómez-Plana Rodríguez (s233165)

Alicia Llorente Herrero (s233658)

Ona Saulianskaite (s232958)

## Introduction 

This repository focuses on investigating how smoking habits and other phenotypic factors influence gene expression in the TCGA-GDC LUAD cohort. These preliminary insights contribute to a further understanding of the impact of smoking on lung adenocarcinoma. Advancing the research on lung cancer is key, since lung cancer is the leading cause of cancer-related death in the world. 


## Data Availability 
The data used is from the[ XenaBrowser from the University of California Santa Cruz]([url](https://xenabrowser.net/datapages/?cohort=GDC%20TCGA%20Lung%20Adenocarcinoma%20(LUAD)&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443)) . The data consists of data from the GDC TCGA Lung Adenocarcinoma (LUAD) cohort. 
The files were downloaded on the 18th of November 2024.

In particular, we used: 

[STAR Counts Data]([url](https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.star_counts.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443)): Log-transformed count matrix containing the counts for the genes tagged by Ensembl IDs. We started the analysis with a total of 589 samples from the cohort. The downloaded version was 05-10-2024. https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.star_counts.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

[Phenotype information about the cohort. ]([url](https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.clinical.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443)). This dataset contains metadata regarding our samples, that was interesting to consider during our analysis since it provided us with additional information regarding the cohort. The downloaded version was 09-07-2024. https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.clinical.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

[ID/Gene mapping file]([url](https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.star_counts.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443)). Since our counts were for Ensembl IDs and we wanted to see the counts for the gene symbols, we downloaded this mapping file, which can be found under ID/Gene Mapping in the link. https://xenabrowser.net/datapages/?dataset=TCGA-LUAD.star_counts.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

## Dependencies
This project makes use of the following packages:
tidyverse
here
DESeq2
ggrepel


## Related Sources

https://pmc.ncbi.nlm.nih.gov/articles/PMC10236141/

https://clauswilke.com/blog/2020/09/07/pca-tidyverse-style/




