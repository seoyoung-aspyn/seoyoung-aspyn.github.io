---
name: World_Mortality_Rate_Viz
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a Final Project Phase 3.1 for IS445 Data Viz class
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Youth at Risk:<br> A Global Overview of Child Mortality Trends
By Seoyoung Yoon, Nicole Gromski, Sahithi Manne 
<br>
<br>
<br>

## About our dataset
This dataset shows the mortality rate for children ages 0-5 for countries across the world. The rows are countries in alphabetical order, and the columns show data about the mortality rate from 1960 to 2022. <br> Not all countries have data for every year, so the line graph only shows data for the years available. <br> <br> We linked two plots: one world map, and one interactive line graph, to create an interactive dashboard that displays the corresponding line plot when a country is pressed on the map. The world map incorporates the mortality rate by country in the most recent year in the dataset, 2022, with a tooltip feature highlighting the country name and the mortality rate with a color-coded legend. The datatypes of those fields are country name is a string, mortality rate is a float, and year is a float. 

<br> 
<br>

## Global View: Under-5 Mortality Rate Insights Dashboard
Click on any country on the map to see a line chart illustrating its child mortality trends over the years!
<br> 
<vegachart schema-url="{{ site.baseurl }}/assets/json/new_chart.json" style="width: 100%"></vegachart>
Our dataset is from "The World Bank" &nbsp; ➭  &nbsp;  {% include elements/button.html link= "https://data.worldbank.org/indicator/SH.DYN.MORT" text="Click here" %}

<div id="vis"></div>

<br> 
<br>

## First Viz: The world map 
The dashboard we have created is to allow users to look at the world map, and get a current picture of child mortality rates around the world. The map ranges from a light green to a dark blue, and the darker the blue gets for a country, that means the child mortality rate for that country is higher.  If we click on a country, we can see the name of the country as well as the child mortality rate of that country as of 2022. Additionally, by clicking on the country, the other view in the dashboard shows a line graph of the countries child mortality rate over time.<br>
<br>


## Second Viz: The line graph
The other graph is an interactive line plot where the fields used in the plot include the same fields as the other graph, country name, mortality rate, and year. Year has temporal encoding, mortality rate has a quantitative encoding since they are numerical values, and country name is nominal since it is a qualitative variable with no specified order. The encoding mark used are a geoshape mark for the world map to illustrate a geographic area while the line graph uses the line mark for the progression throughout the years. The dashboard highlights the most recent data for mortality rate by country to compare the under 5 mortality rates by country and then when a country is pressed, a line graph shows that countries’ under 5 mortality rates through the years 1960-2022.<br> 
<br>
<br> 
<br>
<br> 
<br>

# For contextual datasets
<br>

### 1. Child Mortality Rates in 2022: Under 5 vs. 5 to 14 Years
<vegachart schema-url="{{ site.baseurl }}/assets/json/map_plots.json" style="width: 100%"></vegachart>
Our visualization provides a comparative view of child mortality rates for two distinct age groups: under 5 and from 5 to 14 years old, as recorded in 2022. Through two adjacent interactive maps, viewers can hover over countries to reveal a tooltip with the latest mortality figures, offering a clear and immediate comparison between the vulnerabilities of these age groups. This visualization highlights not only the disparities in child health across different regions but also serves as a vital tool for understanding where improvements have been made and where challenges persist. By presenting these two age brackets side by side, we aim to bring to light the progress in global health initiatives and the areas that require continued focus and action.
<br> 
<br>
<br>
<br> 
<br>
<br>

### 2. A Color-Coded World Map of Global Income Groups
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_map.json" style="width: 100%"></vegachart>
This world map provides a visual overview of the global income landscape, categorized by countries' Gross Domestic Product (GDP). The map is color-coded to differentiate between high, upper-middle, lower-middle, and low-income nations. With intuitive color distinctions, viewers can discern the economic tiers of each country. Hovering over a nation reveals a tooltip with its income group, offering an instant snapshot of its economic status.

<br> 
<br>
<br>
<br> 
<br>
<br>


### Extra. Economic Profiles vs. Child Health
A Comparative Analysis of GDP and Under-5 Mortality
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_mortality_map.json" style="width: 100%"></vegachart>
By laying these maps side by side, we aim to initiate a conversation on how economic factors correlate with child mortality rates. 
This comparison may reveal patterns and provoke questions about the impact of wealth on health, the effectiveness of resource allocation, and the priorities of nations in safeguarding the health of future generations.
<br> 
<br>
<br>
<br> 
<br>
<br>
<br> 
<br>
<br>
<br> 
<br>
<br>



<div class="left">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/_projects/2_World_Mortality_Rate_Viz.md" text="Html code"%}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/IS445_Final3.ipynb" text="Python Analysis" %}
</div>