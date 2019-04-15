README
================

# memer <img src="man/figures/logo.png" align="right" width="120" />

## Overview

memer is a a `tidyverse`-compatible `R` package for creating memes.
Mostly wrappers around `magick` functions.

## Installation

``` r
# Install the development version from GitHub:
# install.packages("devtools")
devtools::install_github("styner/memer")
```

## Usage

``` r
library(memer)
meme_get("DistractedBf") %>% 
  meme_text_distbf("tidyverse", "new R users", "base R")
```

<img src="README_files/figure-gfm/cdistbf-1.png" style="display: block; margin: auto;" />

``` r
meme_get("OprahGiveaway") %>% 
  meme_text_bottom("EVERYONE GETS A %>%!!!", size = 36)
```

<img src="README_files/figure-gfm/oprah-1.png" style="display: block; margin: auto;" />

``` r
meme_get("AmericanChopper") %>%
  meme_text_chopper("Stop calling yourself 'just an R user'!",
                    "But I've never written a package!",
                    "So?? You're still an important part of the community!",
                    "But people who write packages are more important",
                    "NO! All members of the community are valued & deserve respect!")
```

<img src="README_files/figure-gfm/chopper-1.png" width="40%" style="display: block; margin: auto;" />
