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
<br>
Dataset is from... {% include elements/button.html link= "https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="Here" %}

<br>
<vegachart schema-url="{{ site.baseurl }}/assets/json/bfro_reports.json" style="width: 100%"></vegachart>



# Some write-up
<br>

## First Viz: UV Index vs. Visibility Heatmap
Description: This heatmap visualizes the relationship between UV index and visibility. Each cell's color represents the predominant season when a Bigfoot report was made.<br>
Encoding: The X-axis represents the UV Index, binned into 20 intervals, while the Y-axis represents Visibility, also binned into 20 intervals.<br>
Color Scheme: The color encoding is based on the "season" variable. Different shades represent different seasons, making it easier to understand the seasonal distribution of Bigfoot reports.<br>
Data Transformations: The data has been binned for both the UV index and visibility, which helps in better visual representation and understanding of the data distribution.<br>
Interactivity: The plot is interactive with selection.<br>
<br>

## Second Viz: State vs. Wind Speed Heatmap
Description: This heatmap showcases Bigfoot reports categorized by state and wind speed. The color of each cell provides insight into the season during which the report was made.<br>
Encoding: The X-axis represents the various states, while the Y-axis displays the wind speed, which is binned into 60 intervals.<br>
Color Scheme: Just like the previous chart, the color here is based on the "season" variable, with different shades indicating different seasons.<br>
Data Transformations: The wind speed data has been binned into 60 intervals, which simplifies the representation and aids in identifying patterns and trends.<br>
Interactivity: The plot is interactive with filtering based on the selection made in the first plot. It means that selecting a portion of the first plot will filter the data in the second plot to match the selection. This interconnected interactivity allows users to explore relationships between the UV index, visibility, wind speed, and state.


<br>
<div class="left">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/assets/json/bfro_reports.json" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/IS445_HW8.ipynb" text="The Analysis" %}
</div>

