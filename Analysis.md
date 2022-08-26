Analysis
================
Tsunghan Hsieh
2022-08-26

# Summary

This analysis is aiming for identifying aging-associated genes
(biomarkers) in large intestine. The data is subset from
<https://s3.console.aws.amazon.com/s3/buckets/czb-tabula-muris-senis?region=us-west-2&tab=objects>.
The subset data was then filtered and normalized by [my python
script](./scRNA_subsetting.ipynb).

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

# Packages

You can also embed plots, for example:

![](Analysis_files/figure-gfm/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
