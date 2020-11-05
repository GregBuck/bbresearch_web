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


Preliminary results for the 2021 Bristol Bay forecast are posted below for everyone's inspection. Each of these files show the output of the six forecast model in each of the major age classes (1.2, 1.3, 2.2, and 2.3) for each river that we maintain a brood table for. This model output is posted without comment. Later this week research staff will be adding comments to each age/river forecast with our preliminary thoughts regarding model selection. We will be making those annotations in enough time that staff can review them prior to Friday's meeting. Please don't hesitate to contact me if you need help interpreting these files or if you spot any errors. Thanks.


[Kvichak](https://rpubs.com/gbbuck/683725)

[Naknek](https://rpubs.com/gbbuck/683727)

[Alagnak](https://rpubs.com/gbbuck/683731)

[Egegik](https://rpubs.com/gbbuck/683738)

[Ugashik](https://rpubs.com/gbbuck/683743)

[Nushagak](https://rpubs.com/gbbuck/683753)

[Wood](https://rpubs.com/gbbuck/683758)

[Igushik](https://rpubs.com/gbbuck/683763)

[Togiak](https://rpubs.com/gbbuck/683765)


Stacy and Jordan have done the traditional forecast spreadsheets for 2021. They are located on the network here:

S:\REG2\BBsalmon\FORECAST\2021\Traditional Rivers Spreadsheets


I've been working on an interactive dashboard that would allow people to explore the effect of varying lengths of brood table datasets have on forecast model output.
The current working version is [here](https://gregbuck.shinyapps.io/forecast_shiny/). The slider on the input box on the left side of the screen can be used to determine how many years back will be used in the output tabs on the right hand part of the screen. The first output tab shows the raw data and transformed data ('lnFCA' = ln(forecast age), 'lnSIB' = ln(sibling), 'lnRS' = ln(R/S)). The next two tabs display the scatter plot of the data and the residual plot resulting from a linnear regression of the data. The last output tab shows the linear model output. This tab might be difficult to interpret unless you are familiar with R model output. I'm looking for a more user friendly output format.