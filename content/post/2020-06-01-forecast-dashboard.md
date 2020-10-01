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

The first iteration (V1.0) of this effort was written in a Rmarkdown document that generates three outputs for each combination of major age class and model. The outputs are one table and two figures. The table shows the results of model regressions of the most recent 10 years. Included are select regression statistics (R-square and slope p-value) and several measures of model accuracy (absolute deviation, absolute percent error, percent error, arctan percent error) An effort was made to develop this table to have a similar look and content as the spreadsheet summary tables that have been in use for years.

The first graphical output is a scatter plot of the data with a linear regression line added for reference. The second graphical output is the residuals of the linnear regression. Again, this graphical output is similar to what has traditionally been produced in our forecasting spreadsheets. Rmarkdown forecast (v1.0) loaded with the 2019 Kvichak River brood table is archived [here](https://rpubs.com/gbbuck/623012).


PLANNED DEVELOPEMENT (FALL 2020): Version 1.0 is a very lengthy document because it uses a very large number of functions directly in the document. This makes for a very cumbersome for further development due to the size of the document. Best coding practices would dictate that these functions (which are likely to be used across multiple documents) be documented and maintained in an R 'package' either on CRAN or a personal Github repository. I plan to create a functional package of forecast functions and redo this document (V1.1) using that package to make future development easier. Also plannned is a second table (V1.2) that would summarize mean measurement error statistics (MAD, MAPE etc) for the most recent 3 and 5 years in a manner similar to the 'summary' tab in the traditional forecast spreadsheets.


The next major iteration of this effort (V2.0) will be an interactive application that makes use of 
the 'shiny' package. This version is still under construction. I intend to complete the development of this version once I've got a useable Bristol Bay forecasting functions package, a partially functional esample is shown here [here](https://gregbuck.shinyapps.io/forecast_shiny/). In this version the user selects the river, age class, model and length of the dataset to use to return output similar to V1.0.

