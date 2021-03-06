---
title       : Slidify for Pitch
subtitle    : for Shiny App
author      : iris
job         : coursera
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Shiny introduction

Shiny is a platform for creating interactive R programs embedded into a web page

With shiny you can very easily create web input form that calls R and thus your prediction algorithm and displays the results.

Even you don't have the knowledge of R, you can use the shiny app via the web and see the data analysis results.

---

## App Introduction

This shinny app offers a convenient and visual way to see the relationships between all variables of diamonds dataset. 

---

## Dataset Introduction

The diamond dataset mainly studies the  prices and other attributes of almost 54,000 diamonds. The variables include price, carat, cut, color, clarity, x, y, z, depth, and table. You can see the more specific explanation in my github repository.

---

## How to use the app

It's very simple and amazing that you can just adjust some bars and inputs, and you'll see the visual and direct changes caused by these adjustments.

1. such as when we pick price as y and hold it constant, we'll see different variables that have different influcences on price when we pick different Xs.

---

## Example
I'll just give you this example. When it's redudant to write R code and read R code, here with the app, you can simply see the instant presentation of the graph by changing the inputs.

Thank you!


```r
library(knitr)
library(ggplot2)
library(datasets)
data(diamonds)

qplot(carat,price,data=diamonds)
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 

---
