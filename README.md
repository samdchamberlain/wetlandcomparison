
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![Travis-CI Build Status](https://travis-ci.org/samdchamberlain/WetlandComparison.svg?branch=master)](https://travis-ci.org/samdchamberlain/WetlandComparison)

WetlandComparison
=================

This package was used the generate the manuscript "Effect of soil iron content and sediment accretion on methane fluxes from restored wetlands." by Samuel D. Chamberlain et. al. This was my first attempt at a reproducible research example, and it follows the R package structure adapted from Carl Boettiger's template found here: <https://github.com/cboettig/template>. Briefly, the /data folder contains soil and half-hourly eddy covariance files used in the analysis, the /R folder contains scripts used to process data, and the /vignettes folder contains the Markdown and bibiography files used to generate the manuscript, as well as two figure images that were not directly reproducible in R. Additionally, /man and /test folders are standard in R packages but are not particularly relevant to this manuscript as functions are not introduced in this package. They are included anyway to follow convention.

Figure 1 and 7 are not directly reproducible in R, but all other analyses herein are reproducible in this package. Figure 1 was generated in ArcMap using the soil series data downloaded from the USDA Web Soil Survey (<https://websoilsurvey.sc.egov.usda.gov/>), and flux footprints generated from our half-hourly flux data using 2D analytical footprint models described in Detto et al. 2006. Figure 7 was generated using a combined information theory-wavelet time series decomposition using a modification of the MATLAB ProcessNetwork Software found here: <https://github.com/samdchamberlain/ProcessNetwork_Software>. All other analyses in this work are reproducible from the 'manuscript.Rmd' file in the /vignettes folder, and running this file will reproduce this manuscript in its entirety.

Installation
------------

You can install WetlandComparison from github with:

``` r
# install.packages("devtools")
devtools::install_github("samdchamberlain/WetlandComparison")
```

How to Run
----------

Load package into RStudio and open the 'manuscript.Rmd' within the /vignettes folder. Using RStudio, click the 'Knit' button at the top of the console and this manuscript, and analyses herein, will be re-created.
