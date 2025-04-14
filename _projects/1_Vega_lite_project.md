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


# Example including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>

In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.


## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ekonsur2/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

