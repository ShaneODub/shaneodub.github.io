---
title: 'Web scraping with R: 101 years of Irish politics'
author: "Shane O Neill"
date: "05/03/2020"
img: scrape-irish-parliament.jpg
layout: post
tags:
- rvest
- R
- scraping
description: Scraping Irish parliamentary data using R.
---



## How do you scrape data with R?

I'll walk you through the method that I'm familiar with, using the *rvest* package.

First, I'll use *pacman* to install some packages that we'll need.


```r
install.packages("pacman")

pacman::p_load(rvest, dplyr, stringr, tidyr)
```


![plot of chunk deputies]({{ site.url }}/assets/img/scrape-irish-parliament-deputies.png)

In this specific example, there are several elements that I want to extract from each webpage, so I'll download the pages in their entirety before extracing what I need and storing it in a dataframe.


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

## Including Plots

You can also embed plots, for example:

![plot of chunk pressure]({{ site.url }}/assets/img/scrape-irish-parliament-pressure-1.png)

![plot of chunk cars_plot]({{ site.url }}/assets/img/scrape-irish-parliament-cars_plot-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
