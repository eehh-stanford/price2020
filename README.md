
<!-- README.md is generated from README.Rmd. Please edit that file -->

# price2020

This repository contains the data and code for our paper:

> Price, M.H., J.M. Capriles, J. Hoggarth, R.K. Bocinsky, C.E. Ebert,
> and J.H. Jones, (2020). *End-to-end Bayesian analysis of radiocarbon
> dates reveals new insights into lowland Maya demography*. In review.

<!-- Our pre-print is online here: -->

<!-- > Authors, (YYYY). _End-to-end Bayesian analysis of radiocarbon dates reveals new insights into lowland Maya demography_. Name of journal/book, Accessed 20 Apr 2020. Online at <https://doi.org/xxx/xxx> -->

### How to cite

Please cite this compendium as:

> Price, M.H., J.M. Capriles, J. Hoggarth, R.K. Bocinsky, C.E. Ebert,
> and J.H. Jones, (2020). *Compendium of R code and data for End-to-end
> Bayesian analysis of radiocarbon dates reveals new insights into
> lowland Maya demography*. Accessed 20 Apr 2020.

## Contents

The **analysis** directory contains:

  - Scripts for performing the analysis
  - [:file\_folder: data-raw](/analysis/data-raw): Raw data used in the
    analysis.
  - [:file\_folder: data-derived](/analysis/data-derived): Data output
    of the analysis.
  - [:file\_folder: figures](/analysis/figures): Plots and other
    illustrations

## How to run in your broswer or download and run locally

This research compendium has been developed using the statistical
programming language R. To work with the compendium, you will need
installed on your computer the [R
software](https://cloud.r-project.org/) itself and optionally [RStudio
Desktop](https://rstudio.com/products/rstudio/download/).

The [:file\_folder: analysis](/analysis) directory contains the code,
data, and output for Price et al. 2020.

To re-create the analysis, clone this repository, change directories to
it, and please run the following in *R*:

``` r
# install.packages("devtools")
devtools::install()

library("price2020")

list.files("analysis", 
           full.names = TRUE, 
           pattern = "FINAL") %>%
           purrr::walk(source)
```

### Licenses

**Text and figures :**
[CC-BY-4.0](http://creativecommons.org/licenses/by/4.0/)

**Code :** See the [DESCRIPTION](DESCRIPTION) file

**Data :** [CC-0](http://creativecommons.org/publicdomain/zero/1.0/)
attribution requested in reuse

### Contributions

We welcome contributions from everyone. Before you get started, please
see our [contributor guidelines](CONTRIBUTING.md). Please note that this
project is released with a [Contributor Code of Conduct](CONDUCT.md). By
participating in this project you agree to abide by its terms.
