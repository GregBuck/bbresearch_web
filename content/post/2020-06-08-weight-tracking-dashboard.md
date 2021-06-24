---
title: weight tracking dashboard
author: Greg Buck
date: '2021-06-24'
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

The dashboard is divided in half. The left half is designed to give a graphical comparison of current and historical weights and the right half is designed to display selected statistical measures of current and historical weight data. Graphically, I'm currently using boxplots and violin plots from 'ggformula' package. 

Historic dataset used for this dashboard is the 'clean' ASL dataset completed in the fall of 2019 ('fish_clean_with_lookups.csv'. All weights are in lbs.

Link [here](https://rpubs.com/gbbuck/785062).




