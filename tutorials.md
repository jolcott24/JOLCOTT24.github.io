---
layout: page
title: Tutorials
excerpt: "Tutorials"
---

### Creating Spatial Visualizations with R classic (with a few helpful packages)

In this tutorial, I will demonstrate how to create a spatial plot in R using the built-in plot() function. My example will be centered around creating a map of voting proportions by town in the state of Maine, but the code used is applicable to a wide variety of spatial data sets. 

#### Getting your data
The first important step is to create a dataset that has Latitude and Longitudinal values. These values are necessary because they tell the plot() function where to put spatial data points. For my data set, I have a list of town names in Maine and corresponding voting data. The original dataset I have can be accessed at the following [link](/2013_referendum_question_1.csv)

As you can see, I have a bunch of town names with vote totals. As we will see later, it is extremely important to have "Maine" at the end of each city name. This is so, when we convert town names to Latitude and Longitude points, we won't get points for similar town names that are not in Maine (for example Amherst, Massachusetts.) 

Next, lets import the packages we will be using to gather the and plot the spatial data. Run the following code: 

``` install.packages("maps")
install.packages("ggmaps")

library(maps)
library(ggmaps)
```
