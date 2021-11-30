Problem Set 7
================

## GitHub Documents

This is an R Markdown format used for publishing markdown documents to
GitHub. When you click the **Knit** button all R code chunks are run and
a markdown file (.md) suitable for publishing to GitHub is generated.

## Gapminder Code

This code is taken from PS02, which uses the a package called
“gapminder”. This package contains socioeconomic data about countries
from 1952- 2007. Here is the code to set up packages and our dataframe:

``` r
#Loading Packages in
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.0     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   1.4.0     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
library(gapminder)

#Now a bit of wrangling
gapminder_2007 <- gapminder %>% 
  filter(year == 2007)
```
## Gapminder Plot

And here is a scatterplot graph made with the dataframe above :

![](README_files/figure-gfm/plot-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
