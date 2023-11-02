---
name: Bfro_Reports_Viz
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a HW8 for IS445 Data Viz class
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Interactive visualization of Bigfoot reports:
<vegachart schema-url="{{ site.baseurl }}/assets/json/bfro_reports.json" style="width: 100%"></vegachart>


# Search The Data & Methods
Dataset is from... {% include elements/button.html link= "https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="Here" %}


<div class="left">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/assets/json/bfro_reports.json" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/IS445_HW8.ipynb" text="The Analysis" %}
</div>

