
<!-- README.md is generated from README.Rmd. Please edit that file -->

# shinyssdtools

<!-- badges: start -->

[![Lifecycle:
maturing](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)](https://github.com/bcgov/repomountie/blob/master/doc/lifecycle-badges.md)
[![R-CMD-check](https://github.com/bcgov/shinyssdtools/workflows/R-CMD-check/badge.svg)](https://github.com/bcgov/shinyssdtools/actions)
[![DOI](https://joss.theoj.org/papers/10.21105/joss.02848/status.svg)](https://doi.org/10.21105/joss.02848)
<!-- badges: end -->

`shinyssdtools` is a shiny application for fitting Species Sensitivity
Distributions (SSDs) using
[`ssdtools`](https://github.com/bcgov/ssdtools).

## Utilization

The most recent deployed version is available at
<https://bcgov-env.shinyapps.io/ssdtools/>.

To install from [GitHub](https://github.com/bcgov/shinyssdtools) and run
the development version locally use

``` r
# install.packages("devtools")
devtools::install_github("bcgov/shinyssdtools")
shinyssdtools::run_app()
```

## Features

In addition to being a Graphical User Interface to the core
functionality in the [`ssdtools`](https://github.com/bcgov/ssdtools)
package, `shinyssdtools` also provides

-   a bilingual (English/French) interface;
-   generation of R scripts for reproducibility
-   customization and downloads of plots and tables

## Information

For more information including how to cite `shinyssdtools` see [Dalgarno
(2021)](https://doi.org/10.21105/joss.02848).

For a review of `ssdtools` and `shinysddtools` in the context of other
SSD software packages see [Fox et
al. (2021)](https://onlinelibrary.wiley.com/doi/10.1002/etc.4925).

## Assistance

To report bugs/issues/feature requests, please file an
[issue](https://github.com/bcgov/shinyssdtools/issues/).

## Contribution

If you would like to contribute, please see our
[CONTRIBUTING](CONTRIBUTING.md) guidelines.

Please note that this project is released with a [Contributor Code of
Conduct](https://github.com/bcgov/shinyssdtools/blob/master/.github/CONTRIBUTING.md).
By participating in this project you agree to abide by its terms.

## Deployment to `shinyapps.io`

### Manually

Run the `deploy-app.R` script in the scripts directory (after setting
the account argument to be your `shinyapps.io` account name).

### Automatically

If your `shinyapps.io` account name is the same as your GitHub account
name simply make a commit in the master or dev branch and include
`deploy app` in the message (after setting `SHINYAPPS_TOKEN` and
`SHINYAPPS_SECRET` in your repository GitHub secrets). This triggers the
`deploy-app.yml` GitHub action.

## License

The code is released under the Apache License 2.0

Copyright 2021 Province of British Columbia

Licensed under the Apache License, Version 2.0 (the “License”); you may
not use this file except in compliance with the License. You may obtain
a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an “AS IS” BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
