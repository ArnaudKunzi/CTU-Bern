Software developed at CTU Bern
================

In addition to assisting researchers with their research, we also
develop tools to assist with various tasks (primarily statistical and
reporting). In the spirit of open science, we share these tools on
various sharing platforms.

## R packages

R is one of the two main statistical programming languages used at CTU
Bern. During our work, we have developed the following packages for
various tasks.

### [`accrualPlot`](https://github.com/CTU-Bern/accrualPlot) <img src='https://github.com/CTU-Bern/accrualPlot/raw/main/man/figures/logo.png' align="right" height="150">

With `accrualPlot`, it is easy to depict recruitment as a cumulative
incidence curve, a bar plot or to estimate the time point at which a
given number of participants will be been enrolled.

<img src='https://github.com/CTU-Bern/accrualPlot/raw/main/man/figures/README-unnamed-chunk-3-1.png'>

More information on `accrualPlot` is available
[here](https://ctu-bern.github.io/accrualPlot).

### [`btabler`](https://github.com/CTU-Bern/btabler) <img src='https://github.com/CTU-Bern/btabler/raw/main/man/figures/sticker.png' align="right" height="150">

`btabler` is a wrapper around the
[`xtable`](https://cran.r-project.org/web/packages/xtable/) package
allowing more optimized tables for use in LaTeX reports.

<img src='https://github.com/CTU-Bern/btabler/raw/main/vignettes/fig/header.png' class="center">

More information on `btabler` is available
[here](https://ctu-bern.github.io/btabler/).

### [`HSAr`](https://github.com/CTU-Bern/HSAr)

`HSAr` is a by-product of CTU Bern’s involvement in the SNFs [Smarter
Health Case National Research Programme
(NRP74)](http://www.nfp74.ch/en/Pages/Home.aspx). It provides an
approach for creating so-called Hospital Service Areas - aggregated
areas supposed to reflect the patterns of flow from people live to where
they go to hospital. The method is described
[here](https://onlinelibrary.wiley.com/doi/full/10.1111/1475-6773.13275).
(The main repository is [here](https://github.com/aghaynes/HSAr))

### [`kpitools`](https://github.com/CTU-Bern/kpitools) <img src='https://github.com/CTU-Bern/kpitools/raw/main/man/figures/logo.png' align="right" height="150">

Risk based monitoring was introduced as a GCP topic in the ICH GCP
E6(R2) revision with the aim of identifying particularly important risks
to a trial in order to circumvent them earlier and limit their influence
on a given trial. `kpitools` has tools to assist in the calculation and
reporting of such risks (i.e. Key Performance Indicators, KPIs).

More information on `kpitools` is available
[here](https://ctu-bern.github.io/kpitools).

### [`presize`](https://github.com/CTU-Bern/presize) <img src='https://github.com/CTU-Bern/presize/raw/master/man/figures/logo.png' align="right" height="150">

`presize` is a package for precision based sample size calculations.
Rather than having a specific hypothesis to test, a trial might be
rather aimed at estimating the magnitude of a effect and want to have an
estimate with a certain precision (e.g. ‘how wide would my confidence
interval be with so-and-so many participants?’, or ‘how many
participants would be required to attain a confidence interval so
wide?’).

`presize` is available on
[CRAN](https://cran.r-project.org/web/packages/presize) and a
user-friendly, non-programmatic version of the application is available
[here](https://shiny.ctu.unibe.ch/presize/) for those unfamiliar with R.

### R Package universe

CTU Bern also has a so-called
[universe](https://ctu-bern.r-universe.dev), hosted by
[ROpenSci](https://ropensci.org/r-universe/), for easier installation of
our R packages. For packages not on CRAN, and those with versions not
yet posted to CRAN, it allows the installation of packages as if the
packages in the universe were a part of CRAN. For instance, `presize` is
on [CRAN](https://cran.r-project.org/web/packages/presize) but it’s
development version is on [GitHub](https://github.com/CTU-Bern/presize).
The CRAN version of the package can be installed with
`install.packages("presize")`, while the development version must be
installed with `remotes::install_github("CTU-Bern/presize")`. By using
the CTU-Bern universe, it is possible to install the development version
of `presize` via the first syntax. The following code can be used to
tell R to search the CTU Bern universe for a package first and install
it from there if available and if not search CRAN instead (or whatever
repository is mentioned in the second place).

``` r
options(repos = c(ctu = "https://ctu-bern.r-universe.dev",
                  cran = "https://cloud.r-project.org"))
```

`presize`, or any of the packages mentioned above, can then be installed
into R via e.g. `install.packages("presize")`.

As well as the installation of the packages, the universe also has the
vignettes and articles compiled

The `options` code above should be put towards the top of a script or
perhaps in a `.Rprofile` file (typically stored in the Documents or
project folder and is used for setting your personal defaults). See
[here](https://support.rstudio.com/hc/en-us/articles/360047157094-Managing-R-with-Rprofile-Renviron-Rprofile-site-Renviron-site-rsession-conf-and-repos-conf)
for more details.

## Stata

Stata is the second programming language primarily used at CTU Bern.
Again, we have developed various codes that may be of general interest
to users.

### [`btable`](https://github.com/CTU-Bern/btable) <img src='https://github.com/CTU-Bern/btable/raw/main/sticker.png' align="right" height="150">

`btable` makes creating baseline tables simple in Stata. It is a very
flexible approach used by most statisticians at CTU Bern, even those
that primarily use R for their analyses.

### [`stata_secutrial`](https://github.com/CTU-Bern/stata_secutrial)

This repository contains code for reading secuTrial data into Stata and
does a lot of preparatory tasks such as labeling variables and
formatting dates.

## Other packages…

CTU Bern was also actively involved in programming the
[`secuTrialR`](https://github.com/SwissClinicalTrialOrganisation/secuTrialR)
package for loading secuTrial datasets in to R.
