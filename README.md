# Data Visualization with D3.js Project

By: Sruti Jain

Date: 16 May 2017

contact: sruti.j1806@gmail.com

##Deliverables

This repository contains the following project deliverables:

 * index.html -- Code for the data visualization. 
 * data/Final Dataset.csv -- Final data set used for this project
 * data/codebook.md -- Codebook for the data used for this project
 * data/cleaningData.rmd -- R script used for combining data sets and saving the final data in Final Dataset.csv.
 * data/\*.xlsx -- Data sets downloaded from gapminder.org for this project.

##Summary

This visualization aims to showcase that people in most countries increased their daily caloric consumption, as well as average body mass index (BMI) in the years 1998 to 2007.  Each country is indicated as a "bubble" in the visualization, where the size of the bubble is related to that Country's GDP per person.  From the chart, it is apparent that in general the richer countries have the highest daily consumption, as well as the highest BMI, and that the richer countries have increased their consumption the most over the years.  In comparison the poorer countries, especially those in Sub-Saharan Africa, appear to be struggling with food supply. 

##Design

###Goal
My goal with the design of this visualization was to show how, over recent years, most of the world's population has seen an increase in body size in tandem with an increase in food supply, and show how this compares to how "rich" a country is.  If I was doing a static chart, I would probably cherry-pick a small number of countries, create a facet plot, and show a scatterplot of BMI versus calorie consumption, encoding the years as colors on the plot.

However, D3.js has the ability to go beyond the static plots.  So, I chose three variables to plot in bubble plot.  With each bubble corresponding to an individual country, I encoded the x-axis as daily calorie consumption, the y-axis as average BMI, and the size of the bubble as relative to that country's Gross Domestic Product (GDP) per capita.  Then, I knew I wanted to animate through the years, I limited the data to the years 1998-2007.  

###Data

All data from www.gapminder.org

###References

Udacity Data Visualization with D3.js course: https://www.udacity.com/course/ud507

Interactive Data Visualization for the Web. Murray, Scott. Available: http://chimera.labs.oreilly.com/books/1230000000345/

Dimple.js: http://dimplejs.org/index.html . Special mention:

 * Storyboard Control example:http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control
 * Interactive Legend: http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
 * Dimple wiki: https://github.com/PMSI-AlignAlytics/dimple/wiki

D3.js: https://github.com/mbostock/d3/wiki
