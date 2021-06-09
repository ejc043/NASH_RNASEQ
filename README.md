# NASH_RNASEQ
SAMPLES: https://www.ncbi.nlm.nih.gov/gds/?term=GSE129516[ACCN]%20AND%20gsm[ETYP]
each barcode, matrix, and features file for controls1-3 and nash1-3 were found here: https://www.ncbi.nlm.nih.gov/gds/?term=GSE129516[ACCN]%20AND%20gsm[ETYP]
http://128.197.168.11/kkarri/NASH/data/

Because the purpose of this project was to determine differential gene expression of proinflammatory biomarkers, I decided to use processed matrix data over raw FASTQ
files. 
All processed files can be found above. 
I used many resources to determine differential gene expression, including the folloowing:

https://www.youtube.com/watch?v=aZIauqUp0oQ&ab_channel=RebeccaJCarlson
https://pachterlab.github.io/kallistobustools/tutorials/kb_kite/python/kb_kite/
https://chanzuckerberg.github.io/scRNA-python-workshop/preprocessing/00-tabula-muris.html
      
The output of this code are multiple graphs as png files: 
1. violin plot for n_counts of gene and log of n_counts
2. histogram for cell quality controls
3. scatter plot where x axis is mean expression of genes and y axis is dispersion of genes (normalized), where second graph has nonnormalized values on y axis
4. PCA plot of Tnfsf18 
5. UMAP of Tnfsf4, Tnfsf18, Tnfsf10 (similar gene expression)
6. clustering by partitioning N cells into k clusters
7. violin plot of Prex2 and Il17a which exhibit differential expression when computing by leiden algorithm
