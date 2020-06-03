---
title: scheduled event test dashboard
author: Greg Buck
date: '2020-06-02'
slug: scheduled-event-test-dashboard
categories: []
tags:
  - dashboard
description: ''
thumbnail: ''
---

This plot shows daily total cum sockeye count from a mariner query. I'm trying to get query to run at pre-programed
times. Link [here](https://rpubs.com/gbbuck/623123).

To get this to work I will need to set up a scheduled task in the Windows 'Task Scheduler' that will execute the following
tasks in order:  

1. Establish VPN connection.
2. Open Rstudio.
3. Knit .Rmd file.
4. publish HTML output to Rpubs.
5. Close Rstudio.
6. Close VPN connection.

