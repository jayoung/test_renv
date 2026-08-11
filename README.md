
Keep this repo as simple as possible to test knitting and renv and libPaths

## Initialize repo

I'm using Mac Rstudio and R 4.5.3 

Notes on that: I initialized a new Rproject using Rstudio, checking the 'use renv' and 'create git repo' boxes.

Now do this:

```
library("renv")
renv::init()
```

It restarts R, and creates the renv subdir.

Put the project up on github:

Opening an Rmd file triggers installation of the rmarkdown package and dependencies

Clicking 'knit' triggered installation of more packages

If I want to install some packages:
- To install a CRAN package I do something like this: `renv::install("tidyverse")`
- After I install or update packages, and I'm happy that everything runs OK, I lock the setup: `renv::snapshot()`



## script1 - my_subdir/test_renv.Rmd

Running chunks with the 'run' button:
- the working dir is my_subdir
- libPaths has only the two appropriate renv dirs

Running the whole script with the 'knit' button:
