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



<vegachart schema-url="{{ https://vega.github.io/schema/vega-lite/v5.20.1.json }}" style="width: 100%"></vegachart> 

In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.


## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ekonsur2/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

