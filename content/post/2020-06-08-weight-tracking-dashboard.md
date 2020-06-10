---
title: weight tracking dashboard
author: Greg Buck
date: '2020-06-08'
slug: weight tracking-dashboard
categories: []
tags:
  - dashboard
menu:
  main:
    name: Weight dashboard  
description: ''
thumbnail: ''
---

This tracking dashboard queries the FDMS system and retrieves the weight by ocean age data from the current year. **This dashboard is designed to give a near real-time comparison of Weight of 2 & 3-ocean sockeye being collected by our catch samplers with a historical benchmark.** 

The dashboard is divided in half. The left half is designed to give a graphical comparison of current and historical weights and the right half is designed to display selected statistical measures of current and historical weight data. Graphically, I'm currently using boxplots and violin plots from 'ggformula' package. Currently the dash is using 2012 data as a surrogate for 2020 data for the purpose of designing the dashboard. I Will re-set to once we get sufficient samples 2020 samples in the database. The Mean and Std. Deviation of historic and current data are shown on the right half of the screen.

Link [here](https://rpubs.com/gbbuck/625540).


Developments notes for later:

1. Substitute historic data from Mariner for the 'cleaned' ASL dataset completed in fall of 2019. 
2. Source file: 'weight_dashboar.Rmd'


