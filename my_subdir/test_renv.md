my_subdir/test_renv.Rmd script
================
Janet Young

2026-08-11

Show .libPaths()

``` r
.libPaths()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv/renv/library/macos/R-4.5/aarch64-apple-darwin20"                    
    ## [2] "/Users/jayoung/Library/Caches/org.R-project.R/R/renv/sandbox/macos/R-4.5/aarch64-apple-darwin20/4cd76b74"
    ## [3] "/Library/Frameworks/R.framework/Versions/4.5-arm64/Resources/library"

Show working dir

``` r
getwd()
```

    ## [1] "/Users/jayoung/gitProjects/test_renv/my_subdir"

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
    ## [1] stats     graphics  grDevices utils     datasets  methods   base     
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] digest_0.6.39     fastmap_1.2.0     xfun_0.60         knitr_1.51       
    ##  [5] htmltools_0.5.9   rmarkdown_2.31    lifecycle_1.0.5   cli_3.6.6        
    ##  [9] textshaping_1.0.5 systemfonts_1.3.2 compiler_4.5.3    rstudioapi_0.18.0
    ## [13] tools_4.5.3       ragg_1.5.2        evaluate_1.0.5    yaml_2.3.12      
    ## [17] otel_0.2.0        rlang_1.3.0
