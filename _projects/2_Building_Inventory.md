---
name: Building Inventory Visualization
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a HW8 for IS445 Data Viz class
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# # From a dictionary in Altair in Python:
<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inv_chart1.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inv_chart2.json" style="width: 100%"></vegachart>


<div class="left">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/assets/json/building_charts.json" text="The Data" %}
</div>



<div class="right">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/IS445_HW8.ipynb" text="The Analysis" %}
</div>

