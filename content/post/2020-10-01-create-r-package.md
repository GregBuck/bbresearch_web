---
title: create R package
author: Greg Buck
date: '2020-10-01'
slug: create-r-package
categories:
  - R
tags: [R skill]
description: ''
thumbnail: ''
---

To prepare to create an R package, first download and install the 'devtools' package and then set your working directory where you want your package to be created. The package will be created as a subdirectory at this location.


1) set working directory to whatever parent directory you want to create the package under

2) install 'devtools' package

3) use create commannd to create your package directory e.g. create("test.pkg"). R will restart in this directory and create a project of the same name.

4) this should create a subdirectory here: ~test.pkg/R. This is the directory where you put the functions want in your package (use .R files).

5) Your functions each need to be documented using roxygen2 headers in order to generate package documentation

6) Once your functions have basic header information set working directory back to parent directory 

7) create documentation with command document("test.pkg")

8) install package with command install("test.pkg")

9) package should now be loaded. you can check documentation of functions using the usual ?function command and you can run functions to check verify their accuracy.

10) create an empty 'test.pkg' repository on your GitHub account. Add local files to this repository (easiest way is just to drag and drop). 

11) restart Rstudio. Project 'test.pkg' will now be recognized as a Git repository and further changes can be managed from within Rstudio.


Package is now available for use by the public by downloading the package from GitHub and installing. Example:


library(devtools)  
install_github("GregBuck/test.pkg")  
library(test.pkg)