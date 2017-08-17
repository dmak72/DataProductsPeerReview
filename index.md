---
title       : Shiny Application for Statistics on Violent Crime Rates by US States in 1973
subtitle    : 
author      : David M.
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
<style>
.title-slide {
  background-color: #FFFFFF; /* #EDE0CF; ; #CA9F9D*/
}
</style>



## Overview
This application provides a breakdown of the *USArrests* dataset in R. The data set contains statistics, in arrests per 100,000 residents for assault, murder, and rape in each of the 50 US states in 1973. Also given is the percent of the population living in urban areas.

The application provides the user the ability to view the data in several different ways:
> 1. Overall statistics
> 2. Arrest statistics broken down by US states
> 3. Graphical map of the arrest statistics
> 4. Simple prediction of murder arrest rate based on the other variables

---

## Overall Statistics
The application provides a simple way for a user to view the overall statistics of the dataset.

```
## 'data.frame':	50 obs. of  4 variables:
##  $ Murder  : num  13.2 10 8.1 8.8 9 7.9 3.3 5.9 15.4 17.4 ...
##  $ Assault : int  236 263 294 190 276 204 110 238 335 211 ...
##  $ UrbanPop: int  58 48 80 50 91 78 77 72 80 60 ...
##  $ Rape    : num  21.2 44.5 31 19.5 40.6 38.7 11.1 15.8 31.9 25.8 ...
```

```
##      Murder          Assault         UrbanPop          Rape      
##  Min.   : 0.800   Min.   : 45.0   Min.   :32.00   Min.   : 7.30  
##  1st Qu.: 4.075   1st Qu.:109.0   1st Qu.:54.50   1st Qu.:15.07  
##  Median : 7.250   Median :159.0   Median :66.00   Median :20.10  
##  Mean   : 7.788   Mean   :170.8   Mean   :65.54   Mean   :21.23  
##  3rd Qu.:11.250   3rd Qu.:249.0   3rd Qu.:77.75   3rd Qu.:26.18  
##  Max.   :17.400   Max.   :337.0   Max.   :91.00   Max.   :46.00
```

---

## Arrests Statistics by State
The user can view the the states with the highest arrests rates or filter based on selected criteria. For example:

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3-1.png)

---

## Graphical Map 
The user can see a visual display of the arrest statistics on a graphical map. For example:
 ![Caption for the picture.](figure/map.png)

---

## Prediction Modelling
The user can check prediction models for murder arrest rates based on the other variables. For example:

![plot of chunk unnamed-chunk-4](figure/unnamed-chunk-4-1.png)

---

## Prediction Modelling
This simple design any layout of the application allows the user to look at the data from many different perspectives. 

I hope you enjoy using the application!

Thank You!
