
<!-- README.md is generated from README.Rmd. Please edit that file -->

# lehuynh <img src="man/figures/logo.png" width = "175" height = "200" align="right" />

<!-- badges: start -->

[![R-CMD-check](https://github.com/le-huynh/lehuynh/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/le-huynh/lehuynh/actions/workflows/R-CMD-check.yaml)
[![Lifecycle:
stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://lifecycle.r-lib.org/articles/stages.html#stable)
[![DOI](https://zenodo.org/badge/389311777.svg)](https://zenodo.org/doi/10.5281/zenodo.10421410)
<!-- badges: end -->

[Le-Huynh Truc-Ly’s](https://lehuynh.rbind.io/) R Code and Templates

`lehuynh` is an R package comprising a collection of miscellaneous R
functions and templates that I find particularly useful.

This package includes:  
- Functions for graphics, data importation, data transformation, and
general utilities.  
- Templates for Exploratory Analysis, Bayesian modeling, and crafting
scientific manuscripts.

## Installation

`lehuynh` R package can be installed from GitHub with:

``` r
if(!requireNamespace("devtools", quietly = TRUE)) {
 install.packages("devtools")
}
devtools::install_github("le-huynh/lehuynh")
```

This package is also accessible for download via Zenodo with the DOI
[10.5281/zenodo.10421410](https://zenodo.org/doi/10.5281/zenodo.10421410).

### Functions

- `ggsave_elsevier( )`: Save a plot using `ggplot2::ggsave( )`. Plot
  size follows instructions of Elsevier journals.
- `import_data( )`: Imports multiple data files of the same format from
  a specified directory. The output is a *named* list of imported
  objects.
- `import_excel( )`: Imports an Excel file with multiple sheets and
  returns a named list of imported sheets.
- `lehuynh_theme( )`: Personal ggplot2 theme (white background, black
  axis, black text, etc.).
- `MinMaxScaling( )`: Min-max normalization (min = 0, max = 1).
- `new_project( )`: Create a
  [project](https://github.com/SchlossLab/new_project) for reproducible
  purpose.
- `ppc_brms( )`: Plot fitted versus observed values for *brmsfit*
  Objects.
- `tidytuesday( )`: Create a new folder for
  [\#tidytuesday](https://github.com/rfordatascience/tidytuesday)
  challenge.
- `tsi( )`: Calculate TSI (Trophic state index) (Carlson, 1977).

### Templates

- `draft_elsevier`: Creating an Rmarkdown manuscript for Elsevier
  journals
  [(example)](https://github.com/le-huynh/writing_journal_article_in_rmarkdown/tree/master/elsevier).
- `lehuynh_Bayes_brms`: Basic steps to fit, check, and interpret a
  Bayesian model via `brms` package.
- `lehuynh_EA`: Basic steps to do Exploratory Analysis.
