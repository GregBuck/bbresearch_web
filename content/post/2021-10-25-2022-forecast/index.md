---
title: 2021 Forecast
author: Greg Buck
date: '2020-10-29'
slug: []
categories:
  - Data
tags:
  - forecast
description: ''
thumbnail: ''
---


Preliminary results for the 2022 Bristol Bay forecast are posted below for everyone's inspection. 

[Ugashik](https://rpubs.com/gbbuck/826978)

[Egegik](https://rpubs.com/gbbuck/827005)

[Alagnak](https://rpubs.com/gbbuck/827008)

[Kvichak](https://rpubs.com/gbbuck/827019)

[Nushagak](https://rpubs.com/gbbuck/826962)

[Wood](https://rpubs.com/gbbuck/826967)

[Igushik](https://rpubs.com/gbbuck/826953)




Stacy and Jordan have done the traditional forecast spreadsheets for 2021. They are located on the network here:

S:\REG2\BBsalmon\FORECAST\2021\Traditional Rivers Spreadsheets


I've been working on an interactive dashboard that would allow people to explore the effect of varying lengths of brood table datasets have on forecast model output.
The current working version is [here](https://gregbuck.shinyapps.io/forecast_shiny/). The slider on the input box on the left side of the screen can be used to determine how many years back will be used in the output tabs on the right hand part of the screen. The first output tab shows the raw data and transformed data ('lnFCA' = ln(forecast age), 'lnSIB' = ln(sibling), 'lnRS' = ln(R/S)). The next two tabs display the scatter plot of the data and the residual plot resulting from a linnear regression of the data. The last output tab shows the linear model output. This tab might be difficult to interpret unless you are familiar with R model output. I'm looking for a more user friendly output format.