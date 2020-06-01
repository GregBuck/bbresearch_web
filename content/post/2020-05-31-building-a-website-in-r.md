---
title: Building a website in R
author: Greg Buck
date: '2020-05-31'
slug: building-a-website-in-r
categories:
  - R
tags: []
description: ''
thumbnail: ''
---


The [blogdown](https://bookdown.org/yihui/blogdown/) package in R allows for the generating of static-page 
websites using the R language. I've built two of these and unfortunately did not document the process and 
so had to re-learn a bunch of things so I am writing a quick summary of the process while it is still fresh
in my mind.

To build a website with blogdown you will need a [Git](https://github.com/) account as well as a [netlify](https://www.netlify.com/) 
account. In addition to R and Rstudio you need [Git](https://git-scm.com/) installed on your machine. 
To build a webpage in blogdown by definng a project in Rstudio that builds the website locally and that is 
pushed to a Git repository that is linked to a netlify account. The netlify account detects changes made
to the Git repository and triggers a rebuild to incorporate the changes made locally to the deployed site.

As with most things R there are probably several ways to get started here's the process that worked for me:

1. Create a Git repository. Feel free to add a readme, licence file when starting the repository. Do not
create the gitignore file, that will be created later.

2. Locally open the directory above where you want to create the local directory. In explorer right-click on 
this directory and if you have Git installed you should see an option allowing you to open *Git Bash* in that folder.
In Git you want to clone the directory you just created on your local drive. The Git command is *clone*.
Here's an example:  *git clone https://githumb.com/GregBuck/my_website.git*. This will create a directory with
the same name as your Git repository.

3. Open RStudio. make sure you have blogdown package and Hugo installed. With blodgown package added in your
R session you can run *Hugo_install()* command.

4. Now start a new project (File>New Project) and select existing directory option (in this example it would be 
*~/my_website*). This will set the projects working directory to *my_website*.

