---
title: 2020 Togiak Herring ASL
author: Greg Buck
date: '2020-08-03'
slug: 2020-togiak-herring-asl
categories:
  - Data
tags:
  - Herring ASL
description: ''
thumbnail: ''
---


The 2020 Togiak harvest was sampled by getting 6 (?) 50 lb boxes of herring off the M/V Gordan Jensen and shipped through Dillingham to King Salmon where salmon catch samplers worked them up while waiting for salmon processors to get started.

```{r}

library(ggformula)
setwd("~/2020 Herring")
dat <- read.csv("combined.samples.csv")
tmp <- subset(dat,age<28)
gf_boxplot(weight~age, group = ~age, data = tmp)

```

Figure 1. boxplot of 2020 Togiak herring weight at age.


