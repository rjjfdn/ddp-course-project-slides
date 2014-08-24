---
title       : Multivariate Linear Models for mtcars Dataset
subtitle    : Developing Data Products - Course Project
author      : Reinald Kim T. Amplayo
job         : Coursera Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Product Inspiration

- Course Project of Regression Models class
- Makes use of the mtcars dataset
- You create a linear model that has the transmission (am) variable as a predictor and the mpg variable as an outcome
- You interpret the variables correctly and quantify the difference between the two types of transmission in terms of their mpg
- This product helps you answer that course project!

---

## About the mtcars Dataset

- Motor Trend Car Road Tests
- The data was extracted from the 1974 Motor Trend US magazine, and comprises fuel consumption and 10 aspects of automobile design and performance for 32 automobiles (1973-74 models).


```
## 'data.frame':	32 obs. of  11 variables:
##  $ mpg : num  21 21 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 ...
##  $ cyl : num  6 6 4 6 8 6 8 4 4 6 ...
##  $ disp: num  160 160 108 258 360 ...
##  $ hp  : num  110 110 93 110 175 105 245 62 95 123 ...
##  $ drat: num  3.9 3.9 3.85 3.08 3.15 2.76 3.21 3.69 3.92 3.92 ...
##  $ wt  : num  2.62 2.88 2.32 3.21 3.44 ...
##  $ qsec: num  16.5 17 18.6 19.4 17 ...
##  $ vs  : num  0 0 1 1 0 1 0 1 1 1 ...
##  $ am  : num  1 1 1 0 0 0 0 0 0 0 ...
##  $ gear: num  4 4 4 3 3 3 3 4 4 4 ...
##  $ carb: num  4 4 1 1 2 1 4 2 2 4 ...
```

---

## How to Use the Product

1. Choose a combination of features/variables by checking boxes
2. Look at the output, especially the R^2 and the P-values of each variables
3. To check if a feature is helpful, make a plot by choosing a feature and plot it with mpg
4. Go back to 1. until you are satisfied!  

- Very easy! Right?

---

## Next Version Announcements

- We will include multiple datasets, not just mtcars!
- We will include interactions between features! For example, this will be supported, which makes better regression models:


```
##              Estimate Std. Error t value  Pr(>|t|)
## (Intercept) -11.34856   9.397265  -1.208 2.381e-01
## hp            0.22554   0.061874   3.645 1.171e-03
## am           18.66990   3.435923   5.434 1.074e-05
## qsec          2.07791   0.491617   4.227 2.583e-04
## hp:qsec      -0.01599   0.003866  -4.135 3.288e-04
## am:wt        -5.93062   1.294136  -4.583 1.011e-04
```

```
## [1] 0.904
```

- Thank you!
