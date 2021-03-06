---
# Please do not edit this file directly; it is auto generated.
# Instead, please edit 01-BMC_R_Day1_A.md in _episodes_rmd/
title: "General Introduction, Installation and Setup"
author: "Nicholas Ho, Richard Morris, Darya Vanichkina"
keypoints:
- R is a programming language
- RStudio is an integrated development environment which makes working with R easier
objectives:
- Understand the relationship between R and RStudio
- Install all required components
- Describe the purpose of the RStudio Script, Console, Environment, and Plots
questions: What is R? How do we use RStudio to work with R?
source: Rmd
start: 0
teaching: 30
exercises: 0
---



## About R

### The R Programming Language

[R](https://www.r-project.org/) is an open source programming language and software environment for statistical computing and graphics that is supported by the R Foundation for Statistical Computing. Today, it is one of the most popular languages, being used all across the world in a wide variety of domains and fields.

### RStudio

[RStudio](https://www.rstudio.com/) is an integrated development environment (IDE) for R. It includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging and workspace management.

![Example RStudio Screenshot](../fig/RstudioSS.png)

### Installation & Setup

First let's set up the Rstudio panes so that everyone is on the same page.

*Tools* -> *Global Options* -> *Pane Layout*

**Top left:** Console

**Top right:** Source

**Bottom left:** Files, Plots, etc

**Bottom right:** Environment, History, etc


### Starting a new R-project

We'll start a new R-project so we can save our progress and relaunch at anytime.

*File* -> *New Project* -> *New Directory* -> *Empty Project*

We'll call our project "introduction_into_r" and save it in, say, "Documents" folder (or "My Documents" for Windows users)

Note that in "Files", you have a new Rproj file.


### Install prerequisites

Below is a set of commands to install and load packages that you will need for the next three days and also sets some options which will make the course run smoothly. Please copy and run the below commands in your R console.


~~~
#  Install the tidyverse and then load it
install.packages("tidyverse", dependencies = TRUE, repos = "https://cran.csiro.au")
library(tidyverse)

options(scipen = 999)
set.seed(2018)
~~~
{: .language-r}

The `library` command loads all of the functions in the specified library, in this case tidyverse, into our workspace.
