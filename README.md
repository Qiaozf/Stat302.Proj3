[![Travis build status](https://travis-ci.com/Qiaozf/Stat302_Proj3.svg?branch=master)](https://travis-ci.com/Qiaozf/Stat302_Proj3)

[![Codecov test coverage](https://codecov.io/gh/Qiaozf/Stat302_Proj3/branch/master/graph/badge.svg)](https://codecov.io/gh/Qiaozf/Stat302_Proj3?branch=master)

## Installation

To download the Stat302.Proj3 package, use the code below.

``` r
# install.packages("devtools")
devtools::install_github("Qiaozf/Stat302.Proj3")
library(Stat302.Proj3)
```

## Use

The vignette demonstrates example usage of all main functions. Please [file an issue](https://github.com/Qiaozf/Stat302.Proj3/issues) if you have a request for a tutorial that is not currently included. You can see the vignette by using the following code (note that this requires a TeX installation to view properly):


``` r
# install.packages("devtools")
devtools::install_github("Qiaozf/Stat302.Proj3", build_vignette = TRUE, build_opts = c())
library(Stat302.Proj3)
# Use this to view the vignette in the corncob HTML help
help(package = "Stat302.Proj3", help_type = "html")
# Use this to view the vignette as an isolated HTML file
utils::browseVignettes(package = "Stat302.Proj3")
```

Note that R does not allow variable names to start with numbers. Sometimes, when going directly from QIIME2 to phyloseq objects, taxa names will be a large string starting with numbers. To clean these taxa names for use with corncob, use  `clean_taxa_names(my_phyloseq_object)`, see `?clean_taxa_names` for details.

## Status

The preprint describing the corncob methodology is available [here](https://arxiv.org/abs/1902.02776). The manuscript has been accepted to appear in *Annals of Applied Statistics*.

## Bug Reports / Change Requests

If you encounter a bug or would like make a change request, please file it as an issue [here](https://github.com/Qiaozf/Stat302.Proj3/issues).