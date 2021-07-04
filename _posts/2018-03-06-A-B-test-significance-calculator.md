---
layout: post
title: A/B test statistical significance calculator
image: /img/duration-graph.png
tags: [A/B Test, Calculator, R Shiny, Product Analytics, Experiments, Hypothesis Testing, Growth Analytics, Marketing Analytics, Web Analytics, Conversion, Optimisation, p-value]
---

Hypothesis (A/B test) testing is a fundamental part of product analytics. Product owners make decisions based on A/B test results, rather than gut feelings. Once we have the A/B test set up correctly and run it long enough, we want to see whether it has reached statistical significance.  

I’ve finally built my own [R Shiny](https://shiny.rstudio.com/) server and started hosting a simple A/B test statistical significance calculator. The statistical significance calculator is still work in progress, it is currently based on the R code [here](https://github.com/Jverma/Significance-in-A-B-testing). I’ll improve it as soon as I have more time and make it more robust. It shows the p-value and z-score of the hypothesis test and states if the results are statistically significant.
 
You may access the calculator **[here](https://app.gorkemmeral.com/shiny/A-B-test-significance-calculator/)**. 

R Shiny is a great way to create web applications. It’s free to host as well. This A/B test statistical significance calculator is a simple example of what can be done with R Shiny. For more advanced applications visit R Shiny Gallery **[here](https://shiny.rstudio.com/gallery/)**
