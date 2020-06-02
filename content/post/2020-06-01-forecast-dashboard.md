---
title: forecast dashboard
author: Greg Buck
date: '2020-06-01'
slug: forecast-dashboard
categories: [dashboard]
tags:
  - dashboard
description: ''
thumbnail: ''
---

Over the past few years, research staff have been moving our forecast tools from outdated 
spreadsheets which are not very secure, can be prone to errors and very time consuming towards 
a system based on the statistical programming language R. 

The first iteration of this effort was written in a Rmarkdown document that created three 
outputs for each model, a table of linnear regesstion statistics and forecasts for the most 
recent 10-years, a scatterplot of the data and a residual
plot of the dat. An example of the Rmarkdown document run with the current (2019) Kvichak River
brood table can be found [here](https://rpubs.com/gbbuck/623012).

The next iteration of this effort will be an interactive application that makes use of 
the 'shiny' package. This version is still under construction but currently displays the 
selected age & river data and in table format as a scatterplot and residual plot. Currently the 
model output is fixed as the sibling model. Code for the other models has not been incorporated.  
Other models including time series models are planned. Link [here](https://gregbuck.shinyapps.io/forecast_shiny/).

