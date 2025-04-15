---
name: Licenses Visualizations (Homework 5)
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a project that I did using Altair to create visualizations using data on worker licenses in Chicago!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


#  Licenses Visualizations (Homework 5)

This is a project that I did using Altair to create visualizations using data on worker licenses in Chicago!

Example comes from this: https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv

Plot 1
With this bar plot, I am looking at the top 5 most common states where workers in Chicago got their licenses from. I chose dark2 to make each bar clear, since I think that pastel color schemes do not have enough contrast between bars. I encoded a bar plot using data on the top 5 states with the most number of worker licenses given to people working in Chicago. First, I ran value counts for the variable "State" to see how many licenses were given per state, and then found the top 5 states. Then, I plotted a bar chart with the number of licenses in each of the top 5 states using the Altair chart "mark_bar".

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot_1.json" style="width: 100%"></vegachart> 

Plot 2
With this bar plot, I am looking at the number of licenses per status per license type. I used the color scheme category10 for the variable "License Status" because there are many bars, so I wanted to make sure there were a variety of colors in the scheme. As a result, the bars are easy to distinguish between each other, especially nearby bars. Like the other plot, I used the plot mark_bar because "License Status" is a categorical variable. First I made a dataframe with only the columns License Type and License Status. Then I created a new column "count" to see the number number of licenses per type and status. Then, I grouped df_bar by License Type to use for options for the dropdown. I made a dropdown with the variable "License Type" so the user can look at number of licenses per status with their choice for license type. Including bars for all combinations of license status and license type would be very overwhelming compared to showing bars for just one license type at a time, like I am in this bar plot.

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot_2.json" style="width: 100%"></vegachart> 



## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ekonsur2/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

