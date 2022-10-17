# wsl.gbif

wsl.gbif aims at easing the work???ow of retrieving GBIF observations at large spatial scale for all species accepted names and synonyms, and filtering them according to the specific scale of an analysis.

On the one hand, wsl.gbif improves the data accessibility of the rgbif R package (https://cran.r-project.org/web/packages/rgbif/index.html) and allow the whole observations of a given species name (accepted and synonym names) to be retrieved. The user download limit of rgbif is a maximum of 100'000 of species observations in one go. This impends the accessibility to the GBIF database when large observational datasets for many species and region of the world are neededed. wsl.gbif therefore bypasses this limit using rgbif geographic parameters and by adopting a multiple dynamic moving window process allowing to fragment the user's study area of interest to be fragmented in several tiles that always include < 100'000 observations.

On the other hand, wsl.gbif implements easy to use preliminary filtering options implemented during the download so that the user saves some post-processing time of data cleaning. The filetring otpions (n =11) may be chosen independently (or not), and two of them are based on the CoordinateCleaner R package (https://cran.r-project.org/web/packages/CoordinateCleaner/index.html). Additionally, wsl.gbif offers a second function that implements, based on a given species name, a list of all its scientific names (accepted, synonyms, children and related) found in the GBIF backbone taxonomy.

## Installation

You can install the development version from GitHub with:

``` r
remotes::install_github("8Ginette8/wsl.gbif")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
## basic example code
```


## References
