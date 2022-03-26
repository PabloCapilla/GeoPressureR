
<!-- README.md is generated from README.Rmd. Please edit that file -->

# GeoPressureR <img src="man/figures/logo.svg" align="right" height="139" />

<!-- badges: start -->

[![R-CMD-check](https://github.com/Rafnuss/GeoPressureR/workflows/R-CMD-check/badge.svg)](https://github.com/Rafnuss/GeoPressureR/actions)
[![pkgdown](https://github.com/Rafnuss/GeoPressureR/actions/workflows/pkgdown.yaml/badge.svg)](https://github.com/Rafnuss/GeoPressureR/actions/workflows/pkgdown.yaml)
<!-- badges: end -->

The goal of GeoPressureR is to help researcher to analyse pressure
measurement from geolocator. - Part 1: Firstly, it provides a R wrapper
around the [GeoPressure
API](https://github.com/Rafnuss/GeoPressureServer) to query the
probability map using ERA5 pressure. - Part 2: Secondly, using a
mathematical graph, it allows you to model the trajectory producing the
exact probability map at stationary period and simulating paths.

## Installation

You can install the development version of GeoPressureR from
[GitHub](https://github.com/Rafnuss/GeoPressureR) with:

``` r
# install.packages("devtools")
devtools::install_github("Rafnuss/GeoPressureR")
```

## Where to start?

Using the example of a Great Reed Warbler (18LX), the vignettes were
designed to guide you through all the steps with great details.

The vignette [Pressure map](./articles/pressure-map.html) is a good
place to understand the basic workflow used to compute a probability map
from pressure measurement (part 1). It will guide you (or redirect you)
through all the steps from the loading the data, labeling of the
timeseries, querying the ERA5 pressure map and finally computing the
likelihood map.

Once the probability maps are computed, the vignette [Basic
graph](./articles/basic-graph.html) will help you create the graph and
compute three main outputs: (1) the most likely trajectory, (2) the
(posterior) probability map of each stationary period and (3) simulation
of possible path.

## Related Ressources

> Raphaël Nussbaumer, Mathieu Gravey, Felix Liechti Global positioning
> by atmospheric pressure retrieved from multi-sensor geolocators, 25
> February 2022, PREPRINT (Version 1) available at Research Square
> \[<https://doi.org/10.21203/rs.3.rs-1381915/v1>\]

> Raphaël Nussbaumer, Mathieu Gravey, Felix Liechti et al. Improving the
> spatial accuracy of multi-sensor geolocators’ position using
> atmospheric surface pressure. October 2021. *7th International
> Bio-logging Science Symposium*.PRESENTATION available on
> [Youtube](https://www.youtube.com/watch?v=0JsYU_xfKN8).

## Related Code

-   [GeoPressureMAT](https://github.com/Rafnuss/GeoPressureMAT) The
    development of the method was done on MATLAB. Here is the repo with
    all the codes.
-   [GeoPressure API](https://github.com/Rafnuss/GeoPressureServer) This
    is where the core computation with Google Earth Engine is done. You
    can have a look here to see how this is done.
-   [GeoLight](https://github.com/slisovski/GeoLight/tree/Update_2.01) R
    package to analyse light data. We are borrowing some of their
    function (see [`geolight.R`](./reference/index.html#geolight))
-   [PAMLr](https://github.com/KiranLDA/PAMLr): Extensive toolbox to
    analyse multi-sensor geolocator. Several function from this package
    are inspired from this package (see
    [`pam.R`](./reference/index.html#pam-data)).

## Want to contribute?

The code is still in active development. Feel free to [submit an issue
on Github](https://github.com/Rafnuss/GeoPressureR/issues) with
suggetions or bugs
