# Module Gene Analysis Results

## Overview
This folder contains the processed module gene data for the UKB_22q_GWAS project, specifically for the target modules: **magenta**, **lightcyan**, and **skyblue3**.

## Files Description

### Gene Lists (Text Files)
- `magenta_genes.txt` - 817 genes from magenta module
- `lightcyan_genes.txt` - 675 genes from lightcyan module  
- `skyblue3_genes.txt` - 243 genes from skyblue3 module
- `all_target_modules_genes.txt` - Combined unique genes (1,735 total)

### Gene Region Data (CSV Files)
- `gene_regions.csv` - Complete gene region data for all target modules
- `magenta_gene_regions.csv` - Chromosomal regions for magenta module genes
- `lightcyan_gene_regions.csv` - Chromosomal regions for lightcyan module genes
- `skyblue3_gene_regions.csv` - Chromosomal regions for skyblue3 module genes

## Summary Statistics

### Gene Count by Module:
- **Magenta**: 808 genes with chromosomal data
- **Lightcyan**: 667 genes with chromosomal data
- **Skyblue3**: 239 genes with chromosomal data

### Top Chromosomes by Gene Count:
1. Chromosome 1: 165 genes
2. Chromosome 2: 126 genes
3. Chromosome 7: 111 genes
4. Chromosome 19: 108 genes
5. Chromosome 3: 100 genes

## Data Format

### Gene Region CSV Columns:
- `gene_symbol` - Gene name
- `chromosome` - Chromosome number
- `start` - Gene start position
- `end` - Gene end position
- `strand` - DNA strand (+/-)
- `ensembl_id` - Ensembl gene ID
- `biotype` - Gene biotype
- `module` - Module assignment (magenta/lightcyan/skyblue3)

## Analysis Pipeline
1. **Data Extraction**: Extracted genes from `data/module_genes.csv`
2. **Gene Annotation**: Queried Ensembl REST API for chromosomal coordinates
3. **Data Processing**: Created module-specific and combined datasets
4. **Quality Control**: Verified gene counts and chromosomal distribution

## Next Steps
- Use these gene lists for GWAS analysis
- Create chromosomal region plots
- Perform pathway enrichment analysis
- Validate findings in independent datasets

## Date Created
August 5, 2025 