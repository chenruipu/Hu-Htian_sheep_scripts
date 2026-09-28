
# Hu-Htian Sheep Scripts

This repository contains analysis scripts and Jupyter notebooks used for comparative genomic and epigenomic analyses between **Hu sheep (HY)** and **Hetian sheep (HTY)**.

The analyses mainly focus on population structure, SNP analysis, regulatory element identification, chromatin accessibility/histone modification analysis, super-enhancer analysis, transcription factor binding, and GWAS-related variant analysis.

## Repository contents

### `PCA.ipynb`

Analysis and visualization of population genetic structure using principal component analysis (PCA).

Main functions include:

* Principal component analysis
* Visualization of population structure
* Comparison between Hu sheep and Hetian sheep

---

### `SNP.ipynb`

Analysis of SNPs associated with candidate genomic regions and regulatory elements.

The notebook includes procedures for:

* SNP filtering and processing
* Genomic coordinate conversion and organization
* Identification of SNPs located in regulatory regions
* Integration of SNP information with downstream regulatory analyses

---

### `intersect.ipynb`

Genomic interval overlap analysis.

This notebook is used to identify overlaps between genomic features, including:

* H3K27ac peaks
* H3K4me3 peaks
* Enhancers
* Super-enhancers
* SNPs
* Other genomic intervals

The analysis is mainly based on genomic coordinate intersection and filtering.

---

### `peakannotation.ipynb`

Annotation and characterization of ChIP-seq peaks.

The notebook is used for:

* Peak annotation
* Genomic feature classification
* Association of peaks with nearby genes
* Visualization of genomic distributions
* Downstream characterization of H3K27ac and H3K4me3 peaks

---

### `superenhancer.ipynb`

Analysis of **super-enhancers and constituent enhancers** identified from H3K27ac ChIP-seq data.

The updated notebook includes analysis of super-enhancer organization and their associated regulatory features.

Main analyses include:

* Identification and processing of super-enhancers
* Characterization of constituent enhancers
* Comparison of super-enhancers between Hu sheep and Hetian sheep
* Analysis of the number of constituent enhancers within each super-enhancer
* Analysis of super-enhancer genomic characteristics
* Association of super-enhancers with nearby genes
* Comparison of super-enhancer-associated regulatory regions between breeds
* Visualization of super-enhancer distributions and characteristics

The notebook also integrates super-enhancer information with other genomic regulatory features for downstream comparative analysis.

---

### `motifbreakR.ipynb`

Analysis of potential SNP-induced transcription factor binding changes using **motifbreakR**.

The workflow includes:

* Identification of SNPs located in regulatory regions
* Prediction of transcription factor binding motifs
* Evaluation of allele-specific effects on transcription factor binding
* Filtering of potential motif-disrupting SNPs
* Integration with gene expression information
* Identification of candidate regulatory SNP–transcription factor relationships

Expression information can be incorporated to prioritize motif changes occurring in regulatory regions with relevant gene expression patterns.

---

## Analysis workflow

The major analysis workflow can be summarized as:

## Data types

The analyses in this repository integrate several types of genomic data:

* H3K27ac ChIP-seq
* H3K4me3 ChIP-seq
* Enhancer regions
* Super-enhancer regions
* Transcription factor motifs
* Gene annotation
* Genomic interval information

## Software and packages

The analyses were performed using a combination of command-line tools, R, Python, and Jupyter Notebook.

Representative tools and packages include:

* PLINK
* BEDTools
* MACS2 / MACS3
* featureCounts
* HISAT2
* DESeq2
* ChIPseeker
* motifbreakR
* R
* Python
* Jupyter Notebook

Specific software versions and parameters may vary between analyses and are provided in the corresponding notebooks or scripts.

## Genome assembly

Genomic coordinates are based on the sheep reference genome used in the corresponding analysis. Genome assembly information should be kept consistent when performing peak, SNP, enhancer, super-enhancer, and gene annotation analyses.

## Reproducibility

The notebooks in this repository provide the main analysis procedures and visualization code used in the study.

Before running the notebooks, users should modify:

1. Input file paths
2. Reference genome paths
3. Genome annotation files
4. SNP/VCF file paths
5. Peak and enhancer file paths
6. Output directories

Input data are not included in this repository unless explicitly provided.

## Citation

If you use scripts or workflows from this repository, please cite the associated study:

> Chen et al. Comparative genomic and epigenomic analysis of Hu and Hetian sheep.

## Contact

For questions regarding the scripts or analysis workflow, please open an issue in this repository or contact the repository author.
