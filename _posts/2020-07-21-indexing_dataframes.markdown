---
layout: post
title:      "Indexing Dataframes"
date:       2020-07-21 22:52:23 +0000
permalink:  indexing_dataframes
---


Indexing Dataframes in Pandas 

The enitre blog is published on https://medium.com/@menonvid/indexing-dataframes-aecdde4daaf

What is an Index? Index is like an address, which lets us access data points across a dataframe or a series can be accessed. Both Rows and columns have indexes, rows indices are called as index and for columns its their general column names.
Thus, it is extremely important to understand Indexing rows and/or columns. In this tutorial, let’s look at some of the common ways of Indexing in Pandas.

Please install Pandas in case your system doesn’t have it installed.
! pip install pandas

Now let’s get started. Let’s read our data into the dataframe and take a look at it.

**Our Indexing Methods:**

**loc method
iloc method**

The first thing that comes to our mind is ‘the difference between these 2 methods’. Let’s take a small example to understand this. Assume, 5 kids are standing in a line at positions 1 to 5. We have 2 ways of addressing them or calling out to them. Either call them by their name or call them by their position name. If we call the kids by their name, it refers
to as the ‘loc method’ and if we call by the position it refers to as the ‘iloc method’.

**loc Method:**

It is one of the most versatile methods in pandas used to index a dataframe and/or a series method.The loc() function is used to access a group of rows and columns by label(s) or a boolean array. loc[] is primarily label based, but may also be used with a boolean array.

The syntax being:
df.loc[specified rows: specified columns], where df is the name of our dataframe.

The allowed inputs are:
Single label
A list or array of labels
A slice object
A boolean array
A callable function with one argument (the calling Series or DataFrame) and that returns valid output for indexing (one of the above)

**iloc Method:**

iloc returns a Pandas Series when one row is selected, and a Pandas DataFrame when multiple rows are selected, or if any column in full is selected.The iloc method can also be used with both a dataframe and series method. The i in iloc stands for integer, instead of labels.

The syntax for iloc:
df.iloc[<row selection>, <column selection>]

“iloc” is used to select rows and columns by number, in the order that they appear in the data frame. Each row has a row number from 0 to the total number of rows (df.shape[0],0 is for the rows) and iloc[] allows selections based on these numbers. The same applies for columns (ranging from 0 to df.shape[1] , 1 being for columns). There are two ‘arguments’ to iloc — a row selector, and a column selector.
