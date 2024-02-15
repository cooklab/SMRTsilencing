# SMRT-silencing
This repository contains information related to second generation sequencing analysis steps, results, and figures describing short multi-repeat transcript (SMRT)-silencing. 

The pre-print will be deposited on BioRxiv shortly. 

The original description of SMRT silencing was refered to as guide-induced gene silencing. The article is open access and can be found here:
Sharma V.K., Marla S., Zheng W., Mishra D., Huang J., Zhang W., Morris G.P., and D.E. Cook. CRISPR guides induce gene silencing in plants in the absence of Cas. *Genome Biol 23, 6 (2022)*. https://doi-org.er.lib.k-state.edu/10.1186/s13059-021-02586-7



### Results

The relevant data files used for generating Figure 7 from the above manuscript can be found in data, and the code used for analysis and figure generation in notebook. 

The notebook contains code to process the intermediate mapping results contained in the data folder. If you clone the repository, you will need to modify the path to the data directory. If you want to process the data from the original sequencing files, they can be accessed from NCBI SRA, information provided below.

The data for RNA-seq analysis starts after DESeq2 analysis, using Transcript Per Million (TPM) counts and Differential Gene Expression (DGE) analysis. 

The data for small (s)RNA-seq analysis starts after bedtools read depth summary of mapped reads (.bam). 


### Data Availability

The original sequencing data can be accessed from NCBI SRA as follows:

| Sample   | Label       | Replicate | BioProject      |RNA-seq accession | small RNA-seq accession |
|:---------|:------------|:----------|:----------------|:-----------------|:------------------------|
|m3g3      |eGFP.m3g3_8      | one       | PRJNA1015750    | SRR26057916      | SRR26057898           |
|m3g3      |eGFP.m3g3_9      | two       | PRJNA1015751    | SRR26057907      | SRR26057897           |
|m3g3      |eGFP.m3g3.v2_6   | three     | PRJNA1015760    | SRR26057899      | SRR26057905           |
|m6g1      |Egfp m6g1-2_10   | one       | PRJNA1015752    | SRR26057908      | SRR26057901           |
|m6g1      |Egfp m6g1-2.v2_8 | two       | PRJNA1015762    | SRR26057911      | SRR26057903           |
|m6g1      |Egfp m6g1-2.v2_9 | three     | PRJNA1015763    | SRR26057915      | SRR26057912           |
|NT        |Luc-ET_1         | one       | PRJNA1015820    | SRR26057906      | SRR26057913           |
|NT        |Luc-ET_2         | two       | PRJNA1015821    | SRR26057909      | SRR26057914           |
|NT        |Luc-ET_3         | three     | PRJNA1015745    | SRR26057896      | SRR26057910           |
|antisense |eGFP.aseGFPv2_3  | one       | PRJNA1015757    | failed           | SRR26057902           |
|antisense |eGFP.aseGFPv2_4  | two       | PRJNA1015758    | failed           | SRR26057900           |
|antisense |eGFP.aseGFPv2_5  | three     | PRJNA1015759    | failed           | SRR26057904           |

