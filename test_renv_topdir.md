test_renv_topdir.Rmd script
================
Janet Young

2026-08-11

Show .libPaths()

``` r
.libPaths()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv/renv/library/macos/R-4.5/aarch64-apple-darwin20"                    
    ## [2] "/Users/jayoung/Library/Caches/org.R-project.R/R/renv/sandbox/macos/R-4.5/aarch64-apple-darwin20/4cd76b74"

Show working dir

``` r
getwd()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv"

sessionInfo

``` r
sessionInfo()
```

    ## R version 4.5.3 (2026-03-11)
    ## Platform: aarch64-apple-darwin20
    ## Running under: macOS Tahoe 26.6.1
    ## 
    ## Matrix products: default
    ## BLAS:   /Library/Frameworks/R.framework/Versions/4.5-arm64/Resources/lib/libRblas.0.dylib 
    ## LAPACK: /Library/Frameworks/R.framework/Versions/4.5-arm64/Resources/lib/libRlapack.dylib;  LAPACK version 3.12.1
    ## 
    ## locale:
    ## [1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8
    ## 
    ## time zone: America/Los_Angeles
    ## tzcode source: internal
    ## 
    ## attached base packages:
    ## [1] stats     graphics  grDevices datasets  utils     methods   base     
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] compiler_4.5.3  fastmap_1.2.0   cli_3.6.6       htmltools_0.5.9
    ##  [5] tools_4.5.3     yaml_2.3.12     rmarkdown_2.31  knitr_1.51     
    ##  [9] xfun_0.60       digest_0.6.39   rlang_1.3.0     renv_1.2.4     
    ## [13] evaluate_1.0.5
