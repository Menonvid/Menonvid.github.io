---
layout: post
title:      "Data Visualization"
date:       2020-07-08 19:16:21 +0000
permalink:  data_visualization
---


Data Science is a field which focusses on extracting data from various data sets, prepare the data for further analysis and then visualize those data into graphs and findings that makes sense for organizations and groups to make decisions based on those findings.

Visualization is a very important part of Data Science. There are various ways to present the data, so it becomes utmost important to understand which method should be used to present our data.

**Some of the common Data Visualization methods are:**
1. Bar Graph
2. Line Graph
3. Pie Chart
4. Scatter Plot
5. Histogram

The above mentioned methods are the commonly used ways to infer data. But today I want to give a brief intro about **Violin Plot and Strip Plot** charts. How these plots helped me to visualize the set of data I had while working on my project.

**A Violin Plot** is similar to box plot used to plot numeric data but unlike Box Plot, a violin plot helps in understanding the data's distribution. Its important to understand how we read a Violin plot. The thicker part indicates that the values in that area of the violin has higher frequency, and the thinner part implies lower frequency.
Unlike a box plot, in which all of the plot components correspond to actual datapoints, the violin plot features a kernel density estimation of the underlying distribution.

**Defining a Violin Plot :**

sns.violinplot(x=None, y=None, hue=None, data=None, order=None, hue_order=None, bw='scott', cut=2, scale='area', scale_hue=True, gridsize=110, width=0.5, inner='box', split=False, dodge=True, orient=None, linewidth=None, color=None, palette=None, saturation=0.75, ax=None)

Defining some of the commonly used parameters for a Viloin Plot:
x, y, hue :  how the data are plotted , optional
data : dataset for plotting, optional
color : color for all of the elements, optional
order, hue_order : Order to plot the categorical levels in, optional



**A Strip Plot** can be drawn on its own, but it works well  with a box plot or violin plot in cases where we can show all 
observations along with some representation of the underlying distribution.It plots the distribution of variables for each category as individual datapoints. 

**Defining a Strip Plot :**

sns.stripplot(x=None, y=None, hue=None, data=None, order=None, hue_order=None, jitter=True, orient=None, color=None, palette=None, size=5, edgecolor='gray', linewidth=0, ax=None)

Defining some of the commonly used parameters for a Strip Plot:
x, y, hue :  how the data are plotted , optional
data : dataset for plotting, optional
color : color for all of the elements, optional
order, Order to plot the categorical levels in, optional



![](https://github.com/Menonvid/mod1-proj/blob/master/data/ViolinPlot.PNG?raw=true)

