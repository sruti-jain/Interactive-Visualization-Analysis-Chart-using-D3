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

This visualization aims to showcase that people in most countries increased their daily caloric consumption, as well as average body mass index (BMI) in the years 1990 to 2007.  Each country is indicated as a "bubble" in the visualization, where the size of the bubble is related to that Country's GDP per person.  From the chart, it is apparent that in general the richer countries have the highest daily consumption, as well as the highest BMI, and that the richer countries have increased their consumption the most over the years.  In comparison the poorer countries, especially those in Sub-Saharan Africa, appear to be struggling with food supply. 

##Design

###Goal
My goal with the design of this visualization was to show how, over recent years, most of the world's population has seen an increase in body size in tandem with an increase in food supply, and show how this compares to how "rich" a country is.  If I was doing a static chart, I would probably cherry-pick a small number of countries, create a facet plot, and show a scatterplot of BMI versus calorie consumption, encoding the years as colors on the plot.

However, the power of D3.js is the ability to go *beyond* static plots.  So, I chose three variables to plot in a scatterplot, or more specifically a bubble plot.  With each bubble corresponding to an individual country, I encoded the x-axis as daily calorie consumption, the y-axis as average BMI, and the size of the bubble as relative to that country's Gross Domestic Product (GDP) per capita.  Then, I knew I wanted to animate through the years, I limited the data to the years 1990-2007.  

###Data

All data from www.gapminder.org

GDP/capita(US$, inflation-adjusted): https://spreadsheets.google.com/pub?key=0AkBd6lyS3EmpdHo5S0J6ekhVOF9QaVhod05QSGV4T3c&gid=0

Body Mass Index (BMI), men, Kg/m2: https://spreadsheets.google.com/pub?key=0ArfEDsV3bBwCdF9saE1pWUNYVkVsNU1FdW1Yem81Nmc&gid=0

Sugar per person (g per day): https://spreadsheets.google.com/pub?key=phAwcNAVuyj2sdmdhX9zuKg&gid=0

Food supply (kilocalories / person / day): https://spreadsheets.google.com/pub?key=0ArfEDsV3bBwCdGlYVVpXX20tbU13STZyVG0yNkRrZnc&gid=0

World Regions: https://spreadsheets.google.com/pub?key=phT4mwjvEuGBtdf1ZeO7_PQ&gid=1

###References

Udacity Data Visualization with D3.js course: https://www.udacity.com/course/ud507

Dimple.js: http://dimplejs.org/index.html . Special mention:

 * Storyboard Control example:http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control
 * Interactive Legend: http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
 * Custom Tooltips: http://dimplejs.org/adhoc_viewer.html?id=adhoc_bar_custom_tooltips
 * Dimple wiki: https://github.com/PMSI-AlignAlytics/dimple/wiki

D3.js: https://github.com/mbostock/d3/wiki

_Interactive Data Visualization for the Web_. Murray, Scott. Available: http://chimera.labs.oreilly.com/books/1230000000345/

Stackoverflow:
 
 * Several quick syntax checks on www.stackoverflow.com. Did not keep track of all the sites.
 * http://stackoverflow.com/questions/25416063/title-for-charts-and-axes-in-dimple-js-charts