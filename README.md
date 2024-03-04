# Sex-differences-orchestrated-by-androgens-at-single-cell-resolution
Codes provided here are to define the DEGs, AASB-DEGs and significantly enriched biological pathways of each cell type across the 17 tissues.
1. Cellranger_pipeline.sh: The code script in Shell for cellranger pipeline which is executed on Linux System.
2. Data_processing.R: The code in R to perform QC and construct seurat object for downstream analysis.
3. DEG_definition.R: The code in R to define the DEGs between two different conditions (p-adjust < 0.05 and |Log2FC| > 0.5).
4. AASB-DEG_definition.R: The code in R to define androgen-associated sex-biased DEGs (AASB-DEGs) for each cell type across the 17 tissues, which comprises positive AASB-DEGs (the expression levels of which are male-biased and positively associated with androgens) and negative AASB-DEGs (the expression levels of which are female-biased and negatively associated with androgens).
5. Pathway_enrichment.R: The code in R to definine the significantly enriched biological pathways based on DEGs and AASB-DEGs respectively (p < 0.01 & q < 0.01).
# Downloading the data
The raw data for single-cell RNA-seq has been deposited in GSA (https://ngdc.cncb.ac.cn/gsa/) under CRA006610. The processed data for single-cell RNA-seq has been deposited in OMIX (https://ngdc.cncb.ac.cn/omix/) under OMIX001083. 
# Requirements
Cell Ranger (version 6.0.2)
R (version 4.1.0)
Seurat (version 4.0.3)　
DropletUtils (version 1.18.1)　　
DoubletFinder (version 2.0.3)
ggsci (version 2.9)
RColorBrewer (version 1.1-3)
ggplot2 (version 3.4.2)
dplyr (version 1.0.8)
BiocParallel (version 1.28.3)
clustertree (version 0.5.0)
future (version 1.33.0)
clusterProfiler (version 3.12.0)　
org.Mm.eg.db (version 3.8.2)
biomaRt (version 2.40.5)
