# MF9155 Introduction to statistics and bioinformatics for the analysis of large-scale biological data

The environment.yml file contains packages from a course at University of Oslo:

> Introduction to statistics and bioinformatics for the analysis of large-scale biological data
>
> https://www.uio.no/studier/emner/medisin/med/MF9155/

There was one package that was not available as a conda package: `ModelGood`. This package can be installed in R as `install.packages('ModelGood')`.

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

Then run RStudio:
```
rstudio
```

Deactivate environment when you're done:
```
conda deactivate
```

The `list_packages.R` script loads all the packages needed for the course, and runs `devtools::session_info()`.

```
─ Session info ───────────────────────────────────────────────────────────────
 setting  value                       
 version  R version 3.6.1 (2019-07-05)
 os       Ubuntu 18.04.3 LTS          
 system   x86_64, linux-gnu           
 ui       X11                         
 language (EN)                        
 collate  en_US.UTF-8                 
 ctype    en_US.UTF-8                 
 tz       Europe/Oslo                 
 date     2019-11-26                  

─ Packages ───────────────────────────────────────────────────────────────────
 package              * version   date       lib source        
 acepack                1.4.1     2016-10-29 [1] CRAN (R 3.6.1)
 ade4                   1.7-13    2018-08-31 [1] CRAN (R 3.6.1)
 affy                 * 1.62.0    2019-05-02 [1] Bioconductor  
 affyio                 1.54.0    2019-05-02 [1] Bioconductor  
 annotate               1.62.0    2019-05-02 [1] Bioconductor  
 AnnotationDbi        * 1.46.1    2019-08-20 [1] Bioconductor  
 AnnotationFilter       1.8.0     2019-05-02 [1] Bioconductor  
 assertthat             0.2.1     2019-03-21 [1] CRAN (R 3.6.1)
 backports              1.1.5     2019-10-02 [1] CRAN (R 3.6.1)
 base64enc              0.1-3     2015-07-28 [1] CRAN (R 3.6.1)
 Biobase              * 2.44.0    2019-05-02 [1] Bioconductor  
 BiocGenerics         * 0.30.0    2019-05-02 [1] Bioconductor  
 BiocManager          * 1.30.10   2019-11-16 [1] CRAN (R 3.6.1)
 BiocParallel         * 1.18.1    2019-08-06 [1] Bioconductor  
 biomaRt              * 2.40.5    2019-10-01 [1] Bioconductor  
 Biostrings           * 2.52.0    2019-05-02 [1] Bioconductor  
 biovizBase             1.32.0    2019-05-02 [1] Bioconductor  
 bit                    1.1-14    2018-05-29 [1] CRAN (R 3.6.1)
 bit64                  0.9-7     2017-05-08 [1] CRAN (R 3.6.1)
 bitops                 1.0-6     2013-08-17 [1] CRAN (R 3.6.1)
 blob                   1.2.0     2019-07-09 [1] CRAN (R 3.6.1)
 broom                  0.5.2     2019-04-07 [1] CRAN (R 3.6.1)
 BSgenome               1.52.0    2019-05-02 [1] Bioconductor  
 callr                  3.3.2     2019-09-22 [1] CRAN (R 3.6.1)
 cellranger             1.1.0     2016-07-27 [1] CRAN (R 3.6.1)
 checkmate              1.9.4     2019-07-04 [1] CRAN (R 3.6.1)
 cli                    1.1.0     2019-03-19 [1] CRAN (R 3.6.1)
 cluster              * 2.1.0     2019-06-19 [1] CRAN (R 3.6.1)
 codetools              0.2-16    2018-12-24 [4] CRAN (R 3.5.2)
 colorspace             1.4-1     2019-03-18 [1] CRAN (R 3.6.1)
 ConsensusClusterPlus * 1.48.0    2019-05-02 [1] Bioconductor  
 crayon                 1.3.4     2017-09-16 [1] CRAN (R 3.6.1)
 curl                   4.2       2019-09-24 [1] CRAN (R 3.6.1)
 data.table           * 1.12.6    2019-10-18 [1] CRAN (R 3.6.1)
 DBI                    1.0.0     2018-05-02 [1] CRAN (R 3.6.1)
 dbplyr                 1.4.2     2019-06-17 [1] CRAN (R 3.6.1)
 DelayedArray         * 0.10.0    2019-05-02 [1] Bioconductor  
 desc                   1.2.0     2018-05-01 [1] CRAN (R 3.6.1)
 DESeq2               * 1.24.0    2019-05-02 [1] Bioconductor  
 devtools             * 2.2.1     2019-09-24 [1] CRAN (R 3.6.1)
 dichromat              2.0-0     2013-01-24 [1] CRAN (R 3.6.1)
 digest                 0.6.23    2019-11-23 [1] CRAN (R 3.6.1)
 dplR                 * 1.7.0     2019-07-18 [1] CRAN (R 3.6.1)
 dplyr                * 0.8.3     2019-07-04 [1] CRAN (R 3.6.1)
 edgeR                * 3.26.8    2019-09-01 [1] Bioconductor  
 ellipsis               0.3.0     2019-09-20 [1] CRAN (R 3.6.1)
 ensembldb              2.8.1     2019-10-11 [1] Bioconductor  
 fitdistrplus         * 1.0-14    2019-01-23 [1] CRAN (R 3.6.1)
 forcats              * 0.4.0     2019-02-17 [1] CRAN (R 3.6.1)
 foreach                1.4.7     2019-07-27 [1] CRAN (R 3.6.1)
 foreign                0.8-72    2019-08-02 [4] CRAN (R 3.6.1)
 formatR                1.7       2019-06-11 [1] CRAN (R 3.6.1)
 Formula              * 1.2-3     2018-05-03 [1] CRAN (R 3.6.1)
 fs                     1.3.1     2019-05-06 [1] CRAN (R 3.6.1)
 futile.logger        * 1.4.3     2016-07-10 [1] CRAN (R 3.6.1)
 futile.options         1.0.1     2018-04-20 [1] CRAN (R 3.6.1)
 gcrma                * 2.56.0    2019-05-02 [1] Bioconductor  
 genefilter           * 1.66.0    2019-05-02 [1] Bioconductor  
 geneplotter            1.62.0    2019-05-02 [1] Bioconductor  
 generics               0.0.2     2018-11-29 [1] CRAN (R 3.6.1)
 GenomeInfoDb         * 1.20.0    2019-05-02 [1] Bioconductor  
 GenomeInfoDbData       1.2.1     2019-11-25 [1] Bioconductor  
 GenomicAlignments      1.20.1    2019-06-18 [1] Bioconductor  
 GenomicFeatures        1.36.4    2019-07-10 [1] Bioconductor  
 GenomicRanges        * 1.36.1    2019-09-06 [1] Bioconductor  
 GEOquery             * 2.52.0    2019-05-02 [1] Bioconductor  
 getopt                 1.20.3    2019-03-22 [1] CRAN (R 3.6.1)
 ggplot2              * 3.2.1     2019-08-10 [1] CRAN (R 3.6.1)
 glmnet               * 3.0-1     2019-11-15 [1] CRAN (R 3.6.1)
 glue                   1.3.1     2019-03-12 [1] CRAN (R 3.6.1)
 gridExtra              2.3       2017-09-09 [1] CRAN (R 3.6.1)
 gtable                 0.3.0     2019-03-25 [1] CRAN (R 3.6.1)
 Gviz                 * 1.28.3    2019-09-16 [1] Bioconductor  
 haven                  2.2.0     2019-11-08 [1] CRAN (R 3.6.1)
 hgu133plus2.db       * 3.2.3     2019-11-25 [1] Bioconductor  
 Hmisc                * 4.3-0     2019-11-07 [1] CRAN (R 3.6.1)
 hms                    0.5.2     2019-10-30 [1] CRAN (R 3.6.1)
 htmlTable              1.13.2    2019-09-22 [1] CRAN (R 3.6.1)
 htmltools              0.4.0     2019-10-04 [1] CRAN (R 3.6.1)
 htmlwidgets            1.5.1     2019-10-08 [1] CRAN (R 3.6.1)
 httr                   1.4.1     2019-08-05 [1] CRAN (R 3.6.1)
 IRanges              * 2.18.3    2019-09-24 [1] Bioconductor  
 iterators              1.0.12    2019-07-26 [1] CRAN (R 3.6.1)
 jsonlite               1.6       2018-12-07 [1] CRAN (R 3.6.1)
 knitr                  1.26      2019-11-12 [1] CRAN (R 3.6.1)
 lambda.r               1.2.4     2019-09-18 [1] CRAN (R 3.6.1)
 lattice              * 0.20-38   2018-11-04 [4] CRAN (R 3.5.1)
 latticeExtra           0.6-28    2016-02-09 [1] CRAN (R 3.6.1)
 lazyeval               0.2.2     2019-03-15 [1] CRAN (R 3.6.1)
 lifecycle              0.1.0     2019-08-01 [1] CRAN (R 3.6.1)
 limma                * 3.40.6    2019-07-26 [1] Bioconductor  
 locfit                 1.5-9.1   2013-04-20 [1] CRAN (R 3.6.1)
 logging              * 0.10-108  2019-07-14 [1] CRAN (R 3.6.1)
 lsei                 * 1.2-0     2017-10-23 [1] CRAN (R 3.6.1)
 lubridate              1.7.4     2018-04-11 [1] CRAN (R 3.6.1)
 magrittr               1.5       2014-11-22 [1] CRAN (R 3.6.1)
 MASS                 * 7.3-51.4  2019-04-26 [4] CRAN (R 3.6.1)
 Matrix               * 1.2-17    2019-03-22 [4] CRAN (R 3.6.1)
 matrixStats          * 0.55.0    2019-09-07 [1] CRAN (R 3.6.1)
 memoise                1.1.0     2017-04-21 [1] CRAN (R 3.6.1)
 microbenchmark       * 1.4-7     2019-09-24 [1] CRAN (R 3.6.1)
 mnormt                 1.5-5     2016-10-15 [1] CRAN (R 3.6.1)
 ModelGood            * 1.0.9     2014-11-10 [1] CRAN (R 3.6.1)
 modelr                 0.1.5     2019-08-08 [1] CRAN (R 3.6.1)
 munsell                0.5.0     2018-06-12 [1] CRAN (R 3.6.1)
 nlme                   3.1-142   2019-11-07 [4] CRAN (R 3.6.1)
 nnet                   7.3-12    2016-02-02 [4] CRAN (R 3.5.0)
 npsurv               * 0.4-0     2017-10-14 [1] CRAN (R 3.6.1)
 optparse             * 1.6.4     2019-09-16 [1] CRAN (R 3.6.1)
 org.Hs.eg.db         * 3.8.2     2019-11-25 [1] Bioconductor  
 pheatmap             * 1.0.12    2019-01-04 [1] CRAN (R 3.6.1)
 pillar                 1.4.2     2019-06-29 [1] CRAN (R 3.6.1)
 pkgbuild               1.0.6     2019-10-09 [1] CRAN (R 3.6.1)
 pkgconfig              2.0.3     2019-09-22 [1] CRAN (R 3.6.1)
 pkgload                1.0.2     2018-10-29 [1] CRAN (R 3.6.1)
 plyr                   1.8.4     2016-06-08 [1] CRAN (R 3.6.1)
 png                    0.1-7     2013-12-03 [1] CRAN (R 3.6.1)
 preprocessCore         1.46.0    2019-05-02 [1] Bioconductor  
 prettyunits            1.0.2     2015-07-13 [1] CRAN (R 3.6.1)
 processx               3.4.1     2019-07-18 [1] CRAN (R 3.6.1)
 progress               1.2.2     2019-05-16 [1] CRAN (R 3.6.1)
 ProtGenerics           1.16.0    2019-05-02 [1] Bioconductor  
 ps                     1.3.0     2018-12-21 [1] CRAN (R 3.6.1)
 psych                * 1.8.12    2019-01-12 [1] CRAN (R 3.6.1)
 purrr                * 0.3.3     2019-10-18 [1] CRAN (R 3.6.1)
 R.methodsS3            1.7.1     2016-02-16 [1] CRAN (R 3.6.1)
 R.oo                   1.23.0    2019-11-03 [1] CRAN (R 3.6.1)
 R.utils                2.9.0     2019-06-13 [1] CRAN (R 3.6.1)
 R6                     2.4.1     2019-11-12 [1] CRAN (R 3.6.1)
 randomForestSRC      * 2.9.2     2019-11-18 [1] CRAN (R 3.6.1)
 RColorBrewer         * 1.1-2     2014-12-07 [1] CRAN (R 3.6.1)
 Rcpp                   1.0.3     2019-11-08 [1] CRAN (R 3.6.1)
 RCurl                  1.95-4.12 2019-03-04 [1] CRAN (R 3.6.1)
 readr                * 1.3.1     2018-12-21 [1] CRAN (R 3.6.1)
 readxl                 1.3.1     2019-03-13 [1] CRAN (R 3.6.1)
 remotes                2.1.0     2019-06-24 [1] CRAN (R 3.6.1)
 reprex                 0.3.0     2019-05-16 [1] CRAN (R 3.6.1)
 reshape2             * 1.4.3     2017-12-11 [1] CRAN (R 3.6.1)
 rjson                * 0.2.20    2018-06-08 [1] CRAN (R 3.6.1)
 rlang                  0.4.2     2019-11-23 [1] CRAN (R 3.6.1)
 rpart                  4.1-15    2019-04-12 [4] CRAN (R 3.6.1)
 rprojroot              1.3-2     2018-01-03 [1] CRAN (R 3.6.1)
 Rsamtools              2.0.3     2019-10-10 [1] Bioconductor  
 RSQLite                2.1.2     2019-07-24 [1] CRAN (R 3.6.1)
 rstudioapi             0.10      2019-03-19 [1] CRAN (R 3.6.1)
 rtracklayer          * 1.44.4    2019-09-06 [1] Bioconductor  
 rvest                  0.3.5     2019-11-08 [1] CRAN (R 3.6.1)
 S4Vectors            * 0.22.1    2019-09-09 [1] Bioconductor  
 scales                 1.1.0     2019-11-18 [1] CRAN (R 3.6.1)
 seqinr               * 3.6-1     2019-09-07 [1] CRAN (R 3.6.1)
 sessioninfo            1.1.1     2018-11-05 [1] CRAN (R 3.6.1)
 shape                  1.4.4     2018-02-07 [1] CRAN (R 3.6.1)
 signal                 0.7-6     2015-07-30 [1] CRAN (R 3.6.1)
 stringi                1.4.3     2019-03-12 [1] CRAN (R 3.6.1)
 stringr              * 1.4.0     2019-02-10 [1] CRAN (R 3.6.1)
 SummarizedExperiment * 1.14.1    2019-07-31 [1] Bioconductor  
 survival             * 2.44-1.1  2019-04-01 [4] CRAN (R 3.6.1)
 testthat               2.3.0     2019-11-05 [1] CRAN (R 3.6.1)
 tibble               * 2.1.3     2019-06-06 [1] CRAN (R 3.6.1)
 tidyr                * 1.0.0     2019-09-11 [1] CRAN (R 3.6.1)
 tidyselect             0.2.5     2018-10-11 [1] CRAN (R 3.6.1)
 tidyverse            * 1.3.0     2019-11-21 [1] CRAN (R 3.6.1)
 usethis              * 1.5.1     2019-07-04 [1] CRAN (R 3.6.1)
 VariantAnnotation      1.30.1    2019-05-19 [1] Bioconductor  
 vctrs                  0.2.0     2019-07-05 [1] CRAN (R 3.6.1)
 VennDiagram          * 1.6.20    2018-03-28 [1] CRAN (R 3.6.1)
 withr                  2.1.2     2018-03-15 [1] CRAN (R 3.6.1)
 xfun                   0.11      2019-11-12 [1] CRAN (R 3.6.1)
 XML                    3.98-1.20 2019-06-06 [1] CRAN (R 3.6.1)
 xml2                   1.2.2     2019-08-09 [1] CRAN (R 3.6.1)
 xtable                 1.8-4     2019-04-21 [1] CRAN (R 3.6.1)
 XVector              * 0.24.0    2019-05-02 [1] Bioconductor  
 yaml                 * 2.2.0     2018-07-25 [1] CRAN (R 3.6.1)
 zeallot                0.1.0     2018-01-28 [1] CRAN (R 3.6.1)
 zlibbioc               1.30.0    2019-05-02 [1] Bioconductor  

[1] /home/olavur/R/x86_64-pc-linux-gnu-library/3.6
[2] /usr/local/lib/R/site-library
[3] /usr/lib/R/site-library
[4] /usr/lib/R/library
```
