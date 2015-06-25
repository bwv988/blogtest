---
title: Accessing Apache Drill from R
categories: [bigdata, r]
layout: post
---

Over the last decade, the [R](http://www.r-project.org/) programming language has gained a lot of traction outside of its core user base which originates in quantitative research and academia.

The **RedMonk Programming Language survey** -- a survey which aims at analyzing the use of various programming languages by looking at their popularity in GitHub and Stackoverflow -- has recently ranked R in the top quantile in terms of user popularity (see January 2015 [RedMonk ranking](https://redmonk.com/sogrady/2015/01/14/language-rankings-1-15/)).

To frequent users of R this is no real surprise, and it is clear that the popularity of R can largely be attributed to its powerful syntax, built-in support of modern programming paradigms (such as _lambda_ functions or inherent vectorized computations), and its flexibility that supports both quick exploratory analyses as well as complex machine learning algorithms.

However one major disadvantage that standard R suffers from is that computations are limited to data sets that can fit into main memory.

There are now alternative offerings of R ([Microsoft Azure](http://azure.microsoft.com/en-us/), [Revolution R](http://www.revolutionanalytics.com/)) which alleviate the above problem somewhat, but I thought it would be cool :) to try if standard R can be paired with a trending Big Data Query engine, **Apache Drill**, to open up entirely new paths of data access and pre-processing to R.

Although I could not complete my investigation due to other commitments, I did at least manage to connect to Drill and run queries, the data of which is then further processed in R.

Find the code here:

* [GitHub repo](https://github.com/bwv988/apache_drill_and_r)
* `git clone https://github.com/bwv988/apache_drill_and_r.git`

There are also a few slides which document the findings: [Drill and R slides](https://github.com/bwv988/apache_drill_and_r/raw/master/apache_drill.pdf).
