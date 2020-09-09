Report on Gun Murders
================
Rafi Muhammad
10/9/2020

## Introduction

This is a report on 2010 gun murder rates obatain from FBI report

First we are going to use the following library :

``` r
library(tidyverse)
```

    ## -- Attaching packages ---------- tidyverse 1.3.0 --

    ## v ggplot2 3.3.2     v purrr   0.3.4
    ## v tibble  3.0.3     v dplyr   1.0.0
    ## v tidyr   1.1.0     v stringr 1.4.0
    ## v readr   1.3.1     v forcats 0.5.0

    ## -- Conflicts ------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

then, we load data we already wrangled :

``` r
load("rda/murders.rda")
```

we start by generate summary of the data by using sumary() function.
Here is the result :

``` r
summary(murders)
```

    ##     state               abb                      region     population      
    ##  Length:51          Length:51          North Central:12   Min.   :  563626  
    ##  Class :character   Class :character   Northeast    : 9   1st Qu.: 1696962  
    ##  Mode  :character   Mode  :character   South        :17   Median : 4339367  
    ##                                        West         :13   Mean   : 6075769  
    ##                                                           3rd Qu.: 6636084  
    ##                                                           Max.   :37253956  
    ##      total             rate        
    ##  Min.   :   2.0   Min.   : 0.3196  
    ##  1st Qu.:  24.5   1st Qu.: 1.2526  
    ##  Median :  97.0   Median : 2.6871  
    ##  Mean   : 184.4   Mean   : 2.7791  
    ##  3rd Qu.: 268.0   3rd Qu.: 3.3861  
    ##  Max.   :1257.0   Max.   :16.4528

## Murder rate by state

We visualize murder by state data

![](reports_files/figure-gfm/plot_murders-1.png)<!-- -->
