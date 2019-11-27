# MF9155 Introduction to statistics and bioinformatics for the analysis of large-scale biological data

The environment.yml file contains packages from a course at University of Oslo:

> Introduction to statistics and bioinformatics for the analysis of large-scale biological data
>
> https://www.uio.no/studier/emner/medisin/med/MF9155/

## Usage

Create conda environment:
```
conda env create -f MF9155_env.yml
```

If you add something to the file, update the environment:
```
conda env update -f MF9155_env.yml
```

To run R with the installed packages, first activate environment:
```
conda activate MF9155_course
```

Tell RStudio which R path to use:
```
export RSTUDIO_WHICH_R=`which R`
```

Then run RStudio:
```
rstudio
```

Deactivate environment when you're done:
```
conda deactivate
```

## devtools::session_info()

The `list_packages.R` script loads all the packages needed for the course, and runs `sessionInfo()`. Output:

```
R version 3.6.1 (2019-07-05)
Platform: x86_64-pc-linux-gnu (64-bit)
Running under: Ubuntu 18.04.3 LTS

Matrix products: default
BLAS:   /usr/lib/x86_64-linux-gnu/blas/libblas.so.3.7.1
LAPACK: /usr/lib/x86_64-linux-gnu/lapack/liblapack.so.3.7.1

locale:
 [1] LC_CTYPE=en_US.UTF-8       LC_NUMERIC=C              
 [3] LC_TIME=fo_FO.UTF-8        LC_COLLATE=en_US.UTF-8    
 [5] LC_MONETARY=fo_FO.UTF-8    LC_MESSAGES=en_US.UTF-8   
 [7] LC_PAPER=fo_FO.UTF-8       LC_NAME=C                 
 [9] LC_ADDRESS=C               LC_TELEPHONE=C            
[11] LC_MEASUREMENT=fo_FO.UTF-8 LC_IDENTIFICATION=C       

attached base packages:
 [1] grid      parallel  stats4    stats     graphics  grDevices utils    
 [8] datasets  methods   base     

other attached packages:
 [1] microbenchmark_1.4-7        logging_0.10-108           
 [3] dplR_1.7.0                  yaml_2.2.0                 
 [5] rjson_0.2.20                optparse_1.6.4             
 [7] data.table_1.12.6           reshape2_1.4.3             
 [9] forcats_0.4.0               stringr_1.4.0              
[11] dplyr_0.8.3                 purrr_0.3.3                
[13] readr_1.3.1                 tidyr_1.0.0                
[15] tibble_2.1.3                tidyverse_1.3.0            
[17] fitdistrplus_1.0-14         npsurv_0.4-0               
[19] lsei_1.2-0                  MASS_7.3-51.4              
[21] seqinr_3.6-1                rtracklayer_1.44.4         
[23] Gviz_1.28.3                 gcrma_2.56.0               
[25] affy_1.62.0                 Biostrings_2.52.0          
[27] XVector_0.24.0              GEOquery_2.52.0            
[29] biomaRt_2.40.5              hgu133plus2.db_3.2.3       
[31] org.Hs.eg.db_3.8.2          AnnotationDbi_1.46.1       
[33] VennDiagram_1.6.20          futile.logger_1.4.3        
[35] genefilter_1.66.0           psych_1.8.12               
[37] Hmisc_4.3-0                 ggplot2_3.2.1              
[39] Formula_1.2-3               survival_2.44-1.1          
[41] lattice_0.20-38             ModelGood_1.0.9            
[43] randomForestSRC_2.9.2       glmnet_3.0-1               
[45] Matrix_1.2-17               DESeq2_1.24.0              
[47] SummarizedExperiment_1.14.1 DelayedArray_0.10.0        
[49] BiocParallel_1.18.1         matrixStats_0.55.0         
[51] Biobase_2.44.0              GenomicRanges_1.36.1       
[53] GenomeInfoDb_1.20.0         IRanges_2.18.3             
[55] S4Vectors_0.22.1            BiocGenerics_0.30.0        
[57] edgeR_3.26.8                limma_3.40.6               
[59] RColorBrewer_1.1-2          ConsensusClusterPlus_1.48.0
[61] cluster_2.1.0               pheatmap_1.0.12            
[63] BiocManager_1.30.10         devtools_2.2.1             
[65] usethis_1.5.1              

loaded via a namespace (and not attached):
  [1] R.utils_2.9.0            tidyselect_0.2.5         RSQLite_2.1.2           
  [4] htmlwidgets_1.5.1        munsell_0.5.0            codetools_0.2-16        
  [7] preprocessCore_1.46.0    withr_2.1.2              colorspace_1.4-1        
 [10] knitr_1.26               rstudioapi_0.10          GenomeInfoDbData_1.2.1  
 [13] mnormt_1.5-5             bit64_0.9-7              rprojroot_1.3-2         
 [16] vctrs_0.2.0              generics_0.0.2           lambda.r_1.2.4          
 [19] xfun_0.11                biovizBase_1.32.0        R6_2.4.1                
 [22] locfit_1.5-9.1           AnnotationFilter_1.8.0   bitops_1.0-6            
 [25] assertthat_0.2.1         scales_1.1.0             nnet_7.3-12             
 [28] gtable_0.3.0             processx_3.4.1           ensembldb_2.8.1         
 [31] rlang_0.4.2              zeallot_0.1.0            splines_3.6.1           
 [34] lazyeval_0.2.2           acepack_1.4.1            dichromat_2.0-0         
 [37] broom_0.5.2              checkmate_1.9.4          modelr_0.1.5            
 [40] GenomicFeatures_1.36.4   backports_1.1.5          tools_3.6.1             
 [43] affyio_1.54.0            ellipsis_0.3.0           sessioninfo_1.1.1       
 [46] plyr_1.8.4               Rcpp_1.0.3               base64enc_0.1-3         
 [49] progress_1.2.2           zlibbioc_1.30.0          RCurl_1.95-4.12         
 [52] ps_1.3.0                 prettyunits_1.0.2        rpart_4.1-15            
 [55] haven_2.2.0              fs_1.3.1                 magrittr_1.5            
 [58] futile.options_1.0.1     reprex_0.3.0             ProtGenerics_1.16.0     
 [61] pkgload_1.0.2            hms_0.5.2                xtable_1.8-4            
 [64] XML_3.98-1.20            readxl_1.3.1             gridExtra_2.3           
 [67] shape_1.4.4              testthat_2.3.0           compiler_3.6.1          
 [70] crayon_1.3.4             R.oo_1.23.0              htmltools_0.4.0         
 [73] geneplotter_1.62.0       lubridate_1.7.4          DBI_1.0.0               
 [76] formatR_1.7              dbplyr_1.4.2             getopt_1.20.3           
 [79] ade4_1.7-13              cli_1.1.0                R.methodsS3_1.7.1       
 [82] pkgconfig_2.0.3          GenomicAlignments_1.20.1 signal_0.7-6            
 [85] foreign_0.8-72           xml2_1.2.2               foreach_1.4.7           
 [88] annotate_1.62.0          rvest_0.3.5              VariantAnnotation_1.30.1
 [91] callr_3.3.2              digest_0.6.23            cellranger_1.1.0        
 [94] htmlTable_1.13.2         curl_4.2                 Rsamtools_2.0.3         
 [97] lifecycle_0.1.0          nlme_3.1-142             jsonlite_1.6            
[100] desc_1.2.0               BSgenome_1.52.0          pillar_1.4.2            
[103] httr_1.4.1               pkgbuild_1.0.6           glue_1.3.1              
[106] remotes_2.1.0            png_0.1-7                iterators_1.0.12        
[109] bit_1.1-14               stringi_1.4.3            blob_1.2.0              
[112] latticeExtra_0.6-28      memoise_1.1.0           
```
