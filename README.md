# DNAModAnnot_AdditionalData

## Introduction  
This repository contains commands and input files to run an example of 6-methyladenine pattern analysis using the DNAModAnnot package (https://github.com/AlexisHardy/DNAModAnnot).  
To generate the full example report as html or pdf via the DNAModAnnot-protocol-full-analysis.Rmd file, please retrieve all input data and put them in the same directory.  
Then launch the Rmd file in the same directory or modify the paths at the beginning of the Rmd file.

## Input data  

* DNAModAnnot-protocol-full-analysis.Rmd: contains all commands and explanations.  
* contig_list.txt: used for filtering 50 contigs to be used for the analysis.  

The following files were generated from Tetrahymena thermophila SMRT-seq data from GSM2534782 (bax.h5 files):  

* modifications.csv.gz: all sequenced bases (no need to uncompress).  
* modifications.gff.gz: only modified bases (no need to uncompress). 

The following input files must be retrieved from ciliate.org:  

* T_thermophila_June2014_assembly.fasta: genome assembly - http://www.ciliate.org/system/downloads/T_thermophila_June2014_assembly.fasta  
* T_thermophila_June2014.gff3: genome annotation - http://www.ciliate.org/system/downloads/T_thermophila_June2014.gff3  


The following input files must be retrieved from GEO datasets:  

* GSM692081_Growth.map.txt: RNA-seq data - https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM692081  
* GSM2534785_SB210_MNase.120_260.unique.bed: MNase-seq data (must be uncompressed) - https://ftp.ncbi.nlm.nih.gov/geo/samples/GSM2534nnn/GSM2534785/suppl/GSM2534785_SB210_MNase.120_260.unique.bed.gz  
* GSM2534783_WT_H2A.Z_ChIP.120_260.unique.bed: ChIP-seq data (must be uncompressed) - https://ftp.ncbi.nlm.nih.gov/geo/samples/GSM2534nnn/GSM2534783/suppl/GSM2534783_WT_H2A.Z_ChIP.120_260.unique.bed.gz  


## Output data  

The following files can be generated using the Rmd file:

* DNAModAnnot-protocol-full-analysis.html: html report.
* DNAModAnnot-protocol-full-analysis.pdf: pdf report.

The following files are generated by the Rmd file to test the functions adapted to the streaming options from the GViz package:  
  
* scf_8254548Genes.bam: bam file - gene positions and names (scf_8254548 only).    
* scf_8254548Genes.bam.bai: scf_8254548Genes.bam index file.  
* scf_8254548ipdRatio6mA.bw: bigwig file - ipdRatio for 6mAT positions only (scf_8254548 only).   
* scf_8254548ChIPSeq.bw: bigwig file - H2A.Z ChIP-seq coverage (scf_8254548 only).  
* scf_8254548MNaseSeq.bw: bigwig file - H2A.Z ChIP-seq coverage (scf_8254548 only).    

## Citation  
...
