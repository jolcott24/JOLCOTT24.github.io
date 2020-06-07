---
layout: page
title: Tutorials
excerpt: "Tutorials"
---

### Creating Spatial Visualizations with R classic (with a few helpful packages)

In this tutorial, I will demonstrate how to create a spatial plot in R using the built-in plot() function. My example will be centered around creating a map of voting proportions by town in the state of Maine, but the code used is applicable to a wide variety of spatial data sets. 

#### Getting your data
The first important step is to create a dataset that has Latitude and Longitudinal values. These values are necessary because they tell the plot() function where to put spatial data points. For my data set, I have a list of town names in Maine and corresponding voting data. The original dataset I have can be accessed at the following link: 
