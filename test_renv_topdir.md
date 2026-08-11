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

Show environmental variables

``` r
Sys.getenv()
```

    ## __CF_USER_TEXT_ENCODING
    ##                         0x1F6:0x0:0x0
    ## __CFBundleIdentifier    com.rstudio.desktop
    ## CLICOLOR_FORCE          1
    ## COMMAND_MODE            unix2003
    ## DISPLAY                 /var/run/com.apple.launchd.2zqZmHCtl5/org.xquartz:0
    ## DYLD_FALLBACK_LIBRARY_PATH
    ##                         /Library/Frameworks/R.framework/Resources/lib:/Library/Java/JavaVirtualMachines/jdk-11.0.18+10/Contents/Home/lib/server
    ## EDITOR                  vi
    ## GIT_ASKPASS             rpostback-askpass
    ## HOME                    /Users/jayoung
    ## LANG                    en_US.UTF-8
    ## LC_CTYPE                en_US.UTF-8
    ## LN_S                    ln -s
    ## LOGNAME                 jayoung
    ## MAKE                    make
    ## MallocNanoZone          0
    ## MPLENGINE               tkAgg
    ## NOT_CRAN                true
    ## OSLogRateLimit          64
    ## PAGER                   /usr/bin/less
    ## PATH                    /usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/pkg/env/global/bin:/Library/Apple/usr/bin:/opt/X11/bin:/Users/jayoung/perl5/perlbrew/bin:/Users/jayoung/perl5/perlbrew/perls/perl-5.40.2/bin:/opt/homebrew/bin:/Applications/quarto/bin:/Library/TeX/texbin:/usr/texbin:/Applications/RStudio.app/Contents/Resources/app/quarto/bin:/Applications/RStudio.app/Contents/Resources/app/bin/postback
    ## PWD                     /Users/jayoung/gitProjects/test_renv
    ## PYTHONIOENCODING        utf-8
    ## R_ARCH                  
    ## R_BROWSER               /usr/bin/open
    ## R_BZIPCMD               /usr/bin/bzip2
    ## R_CLI_HAS_HYPERLINK_IDE_HELP
    ##                         true
    ## R_CLI_HAS_HYPERLINK_IDE_RUN
    ##                         true
    ## R_CLI_HAS_HYPERLINK_IDE_VIGNETTE
    ##                         true
    ## R_DOC_DIR               /Library/Frameworks/R.framework/Resources/doc
    ## R_GZIPCMD               /usr/bin/gzip
    ## R_HOME                  /Library/Frameworks/R.framework/Resources
    ## R_INCLUDE_DIR           /Library/Frameworks/R.framework/Resources/include
    ## R_LIBS                  /Users/jayoung/gitProjects/test_renv/renv/library/macos/R-4.5/aarch64-apple-darwin20:/Users/jayoung/Library/Caches/org.R-project.R/R/renv/sandbox/macos/R-4.5/aarch64-apple-darwin20/4cd76b74
    ## R_LIBS_SITE             /Library/Frameworks/R.framework/Resources/site-library
    ## R_LIBS_USER             /Users/jayoung/gitProjects/test_renv/renv/library/macos/R-4.5/aarch64-apple-darwin20
    ## R_PAPERSIZE             a4
    ## R_PAPERSIZE_USER        a4
    ## R_PDFVIEWER             /usr/bin/open
    ## R_PLATFORM              aarch64-apple-darwin20
    ## R_PRINTCMD              lpr
    ## R_QPDF                  /Library/Frameworks/R.framework/Resources/bin/qpdf
    ## R_RD4PDF                times,inconsolata,hyper
    ## R_RUNTIME               
    ## R_SESSION_TMPDIR        /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T//Rtmpidhi37
    ## R_SHARE_DIR             /Library/Frameworks/R.framework/Resources/share
    ## R_STRIP_SHARED_LIB      strip -x
    ## R_STRIP_STATIC_LIB      strip -S
    ## R_TEXI2DVICMD           /opt/R/arm64/bin/texi2dvi
    ## R_UNZIPCMD              /usr/bin/unzip
    ## R_ZIPCMD                /usr/bin/zip
    ## RENV_DEFAULT_R_ENVIRON
    ##                         <NA>
    ## RENV_DEFAULT_R_ENVIRON_USER
    ##                         <NA>
    ## RENV_DEFAULT_R_LIBS     <NA>
    ## RENV_DEFAULT_R_LIBS_SITE
    ##                         /Library/Frameworks/R.framework/Resources/site-library
    ## RENV_DEFAULT_R_LIBS_USER
    ##                         /Users/jayoung/Library/R/arm64/4.5/library
    ## RENV_DEFAULT_R_PROFILE
    ##                         <NA>
    ## RENV_DEFAULT_R_PROFILE_USER
    ##                         <NA>
    ## RENV_PROJECT            /Users/jayoung/gitProjects/test_renv
    ## RETICULATE_MINICONDA_PYTHON_ENVPATH
    ##                         /Users/jayoung/gitProjects/test_renv/renv/python/r-reticulate
    ## RMARKDOWN_MATHJAX_PATH
    ##                         /Applications/RStudio.app/Contents/Resources/app/resources/mathjax-27
    ## RMARKDOWN_PREVIEW_DIR   /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T//RtmpwRJwtA
    ## RS_LOG_LEVEL            WARNING
    ## RS_RPOSTBACK_PATH       /Applications/RStudio.app/Contents/Resources/app/bin/rpostback
    ## RS_SHARED_SECRET        fa087c41-04cc-42ea-812d-2aac82acc097
    ## RSTUDIO                 1
    ## RSTUDIO_CHILD_PROCESS_PANE
    ##                         render
    ## RSTUDIO_CLI_HYPERLINKS
    ##                         true
    ## RSTUDIO_CONSOLE_COLOR   256
    ## RSTUDIO_CONSOLE_WIDTH   81
    ## RSTUDIO_DESKTOP_EXE     /Applications/RStudio.app/Contents/MacOS/RStudio
    ## RSTUDIO_FALLBACK_LIBRARY_PATH
    ##                         /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T/rstudio-fallback-library-path-1464267316
    ## RSTUDIO_LONG_VERSION    2026.07.1+147
    ## RSTUDIO_PANDOC          /Applications/RStudio.app/Contents/Resources/app/quarto/bin/tools/aarch64
    ## RSTUDIO_PROGRAM_MODE    desktop
    ## RSTUDIO_SESSION_PID     18913
    ## RSTUDIO_SESSION_PORT    47139
    ## RSTUDIO_USER_IDENTITY   jayoung
    ## RSTUDIO_VERSION         2026.07.1.147
    ## RSTUDIOAPI_IPC_REQUESTS_FILE
    ##                         /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T/RtmpwRJwtA/rstudio-ipc-requests-49e15eb9118d.rds
    ## RSTUDIOAPI_IPC_RESPONSE_FILE
    ##                         /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T/RtmpwRJwtA/rstudio-ipc-response-49e1482f7090.rds
    ## RSTUDIOAPI_IPC_SHARED_SECRET
    ##                         e9d24fd5-312e-48d0-971d-f5b0cd55cc53
    ## SED                     /usr/bin/sed
    ## SF_PARTNER              posit_rstudio
    ## SHELL                   /bin/bash
    ## SHLVL                   0
    ## SPARK_CONNECT_USER_AGENT
    ##                         posit-rstudio
    ## SSH_ASKPASS             rpostback-askpass
    ## SSH_AUTH_SOCK           /var/run/com.apple.launchd.95grgVT0lX/Listeners
    ## TAR                     /usr/bin/tar
    ## TERM                    xterm-256color
    ## TMPDIR                  /var/folders/2y/wndvmd3j0xz24lrl2fjq2j980000gp/T/
    ## TZDIR                   /var/db/timezone/zoneinfo
    ## USER                    jayoung
    ## XPC_FLAGS               0x0
    ## XPC_SERVICE_NAME        application.com.rstudio.desktop.70813624.70813636

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
