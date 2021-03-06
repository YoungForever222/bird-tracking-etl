# UvA-BiTS ETL

## Background

At [the Research Institute for Nature and Forest](http://www.inbo.be), we're tracking large birds as part of [our LifeWatch contribution](http://lifewatch.inbo.be). We are using small solar-powered GPS devices, developed by [UvA-BiTS](http://www.uva-bits.nl). The data are stored in the UvA-BiTS virtual lab and we frequently get a dump from that database on which we work. As tracking data volume grows quicker than human observation data (what we usually work with), we were in need for a data store that contains the cleaned and enriched tracking data in a system that is optimized for querying these *large-ish* data sets. Something like a data warehouse. This R package contains code to extract the data from the UvA-BiTS virtual lab, clean and enrich it, and load it in the data warehouse.

## Install the package

The package is not on CRAN. If you want to use it, download a copy of the code here, and [install it from source](http://stackoverflow.com/questions/1474081/how-do-i-install-an-r-package-from-source). You need a few third party packages, as documented in the package [DESCRIPTION](./DESCRIPTION). R should take care of that. If not, install `lubridate`, `data.table`, `geosphere`, `sp` and `DBI`. If you want to run the tests, you'll need `testthat` too.

## Run the tests

Tests are written using [testthat](https://github.com/hadley/testthat). Run the tests in RStudio by opening the package main directory and pressing CTRL/CMD + SHIFT + T.

## Load the package

```
library(BirdTrackingEtl)
```

## How to use the package

This is explained in the package [vignette](./vignettes/bird-tracking-etl.Rmd).

## Get in touch

Should you encounter issues while using this package, get in touch by [filing an issue](https://github.com/LifeWatchINBO/bird-tracking-etl/issues).
