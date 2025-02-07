# OBiroi Gene models

This repository contains code and some input files for the creation of OBiroi gene models in ["Heterozygosity at a conserved candidate sex determination locus is associated with female development in the clonal raider ant"](https://www.biorxiv.org/content/10.1101/2025.01.24.634795v1.abstract)

## Short read data.

Short read data was processed following the workflow described in Illumina/StringTie_NoGTF/report/WorkflowDescription.html.

This includes Hisat2 alignment and stringtie creation of gene models.

## Long read data

Long read data was processed following the workflow described in PacBio/PBTools/report/WorkflowDescription.html.

This describes the minimap2, isoseq3 and pigeon software steps for creation of gene models.

Additionally a stringtie set of gene models was created following script in PacBio/stringtie/Stringtie_Long.Rmd

## Aggregating Short,Long read data with piRNA and miRNA predictions.

Gene models were aggregated across Short and Long read data following the script shown in CombiningAndCleaning/CombiningAndCleaningUpGTF.html.

The final gene models were integrated with previous OBiroi annotation from RefSeq and finally with miRNA and piRNA predictions.

QC and annotation by Squati/Busco/gffcompare are also described in this document.
