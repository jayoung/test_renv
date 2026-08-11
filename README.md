# test_renv

Goal:  testing renv and Rstudio and knit

Keep this repo as simple as possible to test knitting and renv and libPaths

# Script notes

## script 1 - test_renv_topdir.md

Running chunks with the 'run' button:
- the working dir is the top dir
- libPaths has only the two appropriate renv dirs

Running the whole script with the 'knit' button:
- the working dir is the top dir
- libPaths has only the two appropriate renv dirs



## script 2 - my_subdir/test_renv.Rmd

Running chunks with the 'run' button:
- the working dir is my_subdir
- libPaths has only the two appropriate renv dirs

Running the whole script with the 'knit' button:
- the working dir is my_subdir
- libPaths has the two appropriate renv dirs BUT ALSO:
    `## [3] "/Library/Frameworks/R.framework/Versions/4.5-arm64/Resources/library"`


## script 3 - my_subdir/test_renv_subdir.withLibraryCall.Rmd

Same as my_subdir/test_renv.Rmd but with `library(renv)` added

Running chunks with the 'run' button:
- the working dir is my_subdir
- libPaths has only the two appropriate renv dirs

Running the whole script with the 'knit' button:
- the working dir is my_subdir
- libPaths has only the two appropriate renv dirs

# Rprofile files

This is true on mac and server.
- when I knit a script in the subdir, it reads ~/.Rprofile and NOT the project/.Rprofile
- when I knit a script in the topdir, it reads project/.Rprofile

The renv/activate.R script is sourced via project/.Rprofile so it doesn't get read for scripts that are knit from within subdirs

knit pulldown - set to 'knit directory = project directory'

## original setup

### initialize the R project

I'm using Mac Rstudio and R 4.5.3 

Notes on that: I initialized a new Rproject using Rstudio, checking the 'use renv' and 'create git repo' boxes.

Now do this:

```
library("renv")
renv::init()
```

It restarts R, and creates the renv subdir.

### git stuff

First sync local repo:
```
git add --all .
git commit -m 'first commit'
```

Then installed `gh` command line github tool and do `gh auth login`

Now create repo on github.com: `gh repo create`

Now push the local repo up to github.com
```
git branch -M main
git push -u origin main
```


Opening an Rmd file triggers installation of the rmarkdown package and dependencies

Clicking 'knit' triggered installation of more packages

If I want to install some packages:
- To install a CRAN package I do something like this: `renv::install("tidyverse")`
- After I install or update packages, and I'm happy that everything runs OK, I lock the setup: `renv::snapshot()`

