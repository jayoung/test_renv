my_subdir/test_renv_subdir.withLibraryCall.Rmd script
================
Janet Young

2026-08-11

``` r
library(renv)
```

    ## 
    ## Attaching package: 'renv'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     embed, update

    ## The following objects are masked from 'package:utils':
    ## 
    ##     history, upgrade

    ## The following objects are masked from 'package:base':
    ## 
    ##     autoload, load, remove, use

Show .libPaths()

``` r
.libPaths()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv/renv/library/macos/R-4.6/aarch64-apple-darwin23"                    
    ## [2] "/Users/jayoung/Library/Caches/org.R-project.R/R/renv/sandbox/macos/R-4.6/aarch64-apple-darwin23/46003b10"

Show working dir

``` r
getwd()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv/my_subdir"

sessionInfo

``` r
sessionInfo()
```

    ## R version 4.6.1 (2026-06-24)
    ## Platform: aarch64-apple-darwin23
    ## Running under: macOS Tahoe 26.6.1
    ## 
    ## Matrix products: default
    ## BLAS:   /Library/Frameworks/R.framework/Versions/4.6/Resources/lib/libRblas.0.dylib 
    ## LAPACK: /Library/Frameworks/R.framework/Versions/4.6/Resources/lib/libRlapack.dylib;  LAPACK version 3.12.1
    ## 
    ## locale:
    ## [1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8
    ## 
    ## time zone: America/Los_Angeles
    ## tzcode source: internal
    ## 
    ## attached base packages:
    ## [1] stats     graphics  grDevices utils     datasets  methods   base     
    ## 
    ## other attached packages:
    ## [1] renv_1.2.4
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] compiler_4.6.1    fastmap_1.2.0     cli_3.6.6         tools_4.6.1      
    ##  [5] htmltools_0.5.9   otel_0.2.0        rstudioapi_0.19.0 yaml_2.3.12      
    ##  [9] rmarkdown_2.31    knitr_1.51        xfun_0.60         digest_0.6.39    
    ## [13] rlang_1.3.0       evaluate_1.0.5
