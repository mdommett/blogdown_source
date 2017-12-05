---
title: "Getting to grips with MySQL"
author: ~
date: '2017-12-05'
#image: "post/2hc.mp4"
slug: getting-to-grips-with-mysql
categories: []
tags: 
---

Over the last few months I have been using MySQL to locally archive, store, and access data for a few of my projects. Previously, I was using Excel for this purpose, but I have come to find it less than ideal, mainly due to its clunkiness and the fact that I got into bad habits (no vesion control, poor formatting, rudimentary analyses). As such, I decided to switch to a combination of MySQL and python with pandas.

The data I am analysing come from a variety of test files outputs, namely electronic structure codes [Gaussian](gaussian.com), [Turbomole](http://www.turbomole.com/), and [Molcas](http://www.molcas.org/). I am interested in studying the relaxation mechanisms in molecular rotors, in particular for studying non-radiative decay via intersystem-crossings. However, the exact application is not the focus here, more the process in data extraction and analysis.

First I needed to design my database; I used a column for each spin state and geometry, and level of theory, resulting in 21 columns. Each feature would be a molecular system at a given level of theory.

All of the data can be found herey(LINK). I wrote a python script `fill_db.py`, which mined each output file and filled in each table. Important here was a naming convention for the output files (24 in total). Each function in `fill_db.py` is specifically for a type of output file and type of data to be extracted. As such, is is quite specific for the current task has limited flexibility. However, its still useful as a proof of concept.

Once the database is filled, I use Jupyter and pandas to analyse the data. An exemplar notebook can be found in the repository(LINK). Here I can compare different methods, plotting and analysing using pandas, numpy and matplotlib. Here I am mostly interested in comparing different features (methods), which the database allows well. Once converted to a dataframe in pandas, I can then append new data directly to the dataframe in the notebook, before adding directly to the SQL database.

md





