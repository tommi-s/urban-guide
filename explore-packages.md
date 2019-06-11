explore-packages.R
================
TSVV
2019-06-11

``` r
.libPaths()
```

    ## [1] "C:/Users/TSVV/Documents/R/win-library/3.5"        
    ## [2] "C:/Program Files/Microsoft/R Open/R-3.5.3/library"

``` r
library( tidyverse )
```

    ## -- Attaching packages ---------------------------------- tidyverse 1.2.1 --

    ## v ggplot2 3.1.1       v purrr   0.3.2  
    ## v tibble  2.1.1       v dplyr   0.8.0.1
    ## v tidyr   0.8.3       v stringr 1.4.0  
    ## v readr   1.3.1       v forcats 0.4.0

    ## -- Conflicts ------------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
ipt <- installed.packages() %>%
  as_tibble() %>%
  select( Package, LibPath, Version, Priority, Built )

ipt
```

    ## # A tibble: 152 x 5
    ##    Package    LibPath                                Version Priority Built
    ##    <chr>      <chr>                                  <chr>   <chr>    <chr>
    ##  1 askpass    C:/Users/TSVV/Documents/R/win-library~ 1.1     <NA>     3.5.3
    ##  2 assertthat C:/Users/TSVV/Documents/R/win-library~ 0.2.1   <NA>     3.5.3
    ##  3 backports  C:/Users/TSVV/Documents/R/win-library~ 1.1.4   <NA>     3.5.3
    ##  4 base64enc  C:/Users/TSVV/Documents/R/win-library~ 0.1-3   <NA>     3.5.2
    ##  5 BH         C:/Users/TSVV/Documents/R/win-library~ 1.69.0~ <NA>     3.5.2
    ##  6 bitops     C:/Users/TSVV/Documents/R/win-library~ 1.0-6   <NA>     3.5.2
    ##  7 broom      C:/Users/TSVV/Documents/R/win-library~ 0.5.2   <NA>     3.5.3
    ##  8 callr      C:/Users/TSVV/Documents/R/win-library~ 3.2.0   <NA>     3.5.3
    ##  9 caTools    C:/Users/TSVV/Documents/R/win-library~ 1.17.1~ <NA>     3.5.3
    ## 10 cellranger C:/Users/TSVV/Documents/R/win-library~ 1.1.0   <NA>     3.5.3
    ## # ... with 142 more rows
