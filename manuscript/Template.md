---
title: "Template R Markdown"
author: "Amanda Suzzi"
date: "7/5/2022"
output:
  html_document: 
    keep_md: yes
    toc: yes
    number_sections: yes
    df_print: kable
bibliography: grateful-refs.bib
---




Isolate each computationally demanding step in its own script and write the precious object to file with saveRDS(my_precious, here("results", "my_precious.rds")). Now you can develop scripts to do downstream work that reload the precious object via my_precious <- readRDS(here("results", "my_precious.rds")). Breaking an analysis i
 
# Introduction

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.



# Methods
We used R version 4.1.2 [@base] and the following R packages: grateful v. 0.1.11 [@grateful], knitr v. 1.39 [@knitr2014; @knitr2015; @knitr2022], rmarkdown v. 2.14 [@rmarkdown2018; @rmarkdown2020; @rmarkdown2022].

# Results


```r
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```


You can also embed plots, for example:

![](Template_files/figure-html/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

## Tips
Clean out your workspace and restart R and re-run everything periodically, if things get weird.

Keep things machine- and human-readable, whenever possible.


```r
## insert your brilliant WORKING code here
```


# References
