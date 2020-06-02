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

3. Now start a new project (File>New Project) and select existing directory option (in this example it would be 
*~/my_website*). This will set the project working directory to *my_website*.

4. Open RStudio. make sure you have blogdown package and Hugo installed. With blodgown package added in your
R session you can get Hugo by running the *Hugo_install()* command.

5. Before building your initial site, it is best to spend some time thinking about what kind of layout you want.
A collection of free Hugo templates can be found [here](https://themes.gohugo.io/). Hugo templates range from the 
easy to install and use to the very complex and obtuse. Be prepared to try out several before you settle.

6. Once you have a theme, a new site can be generated with one command:   
          *new_site(theme = "mikemarvel/awesome-theme", theme_example = TRUE)*  
where 'Mikemarvel/awesome-theme' is the Git repository of the theme you want. This will generate the theme example 
For some reason the Git implementation in Rstudio canreally choke on large Git pushes so I'd recommend that 
this first commit be done directly in Git Bash. Close R and open Git Bash in your 'my_website' directory. You will need to
stage everything in this folder, commit everything staged and then push to Git. The commands are:  
          *git add .*  
          *git commit -m "initial commit"*  
          *git push https://github.com/GregBuck/my_website*  

7. In Netlify you need to deploy your website from your Git repository. Once you have created your account you create a 
website from a Git repository. Specify the /public folder in your repository. This is where the static HTML pages that Hugo
creates live.

8. In Rstudio you can create new content. In most themes there is a */content* folder that contains most of the content you
will be interested in customizing. of your website project. Any changes you make can be Git pushed straight
from Rstudio and as the Netlify robots detect new commits their Hugo robots rebuild and redeploy your website. Here's a [tutorial](https://alison.rbind.io/post/2017-06-12-up-and-running-with-blogdown/) I found helpful. Also see [here](https://bookdown.org/yihui/blogdown/rstudio-ide.html) for information about how to use Rstudio addins like 'new post'.

