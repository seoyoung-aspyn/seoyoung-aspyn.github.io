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

# Some write-up : About our dataset
<br>
This dataset shows the mortality rate for children ages 0-5 for countries across the world. The rows are countries in alphabetical order, and the columns show data about the mortality rate from 1960 to 2022. Not all countries have data for every year, so the line graph only shows data for the years available. We linked two plots: one world map, and one interactive line graph, to create an interactive dashboard that displays the corresponding line plot when a country is pressed on the map. The world map incorporates the mortality rate by country in the most recent year in the dataset, 2022, with a tooltip feature highlighting the country name and the mortality rate with a color-coded legend. The datatypes of those fields are country name is a string, mortality rate is a float, and year is a float. 

<br> 

## Interactive visualization of Child Mortality Rate:
<br>
Dataset is from... {% include elements/button.html link= "https://data.worldbank.org/indicator/SH.DYN.MORT" text="Here" %}

<vegachart schema-url="{{ site.baseurl }}/assets/json/new_chart.json" style="width: 100%"></vegachart>

<div id="vis"></div>

<br> 

## First Viz: Worldmap 
<br> 
Description: 
The dashboard we have created is to allow users to look at the world map, and get a current picture of child mortality rates around the world. The map ranges from a light green to a dark blue, and the darker the blue gets for a country, that means the child mortality rate for that country is higher.  If we click on a country, we can see the name of the country as well as the child mortality rate of that country as of 2022. Additionally, by clicking on the country, the other view in the dashboard shows a line graph of the countries child mortality rate over time.<br>
<br>

## Second Viz: The line graph
<br>
Description: 
The other graph is an interactive dropdown line plot where the fields used in the plot include the same fields as the other graph, country name, mortality rate, and year. Year has ordinal encoding since the variables have a chronological order, mortality rate has a quantitative encoding since they are numerical values, and country_name is nominal since it is a qualitative variable with no specified order. The encoding mark used are a geoshape mark for the world map to illustrate a geographic area while the line graph uses the line mark for the progression throughout the years. The dashboard highlights the most recent data for mortality rate by country to compare the under 5 mortality rates by country and then when a country is pressed, a line graph shows that countries’ under 5 mortality rates through the years 1960-2022.<br> 

<br>

# For contextual datasets
<br>

### 1. Viz for world GDP data
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_map.json" style="width: 100%"></vegachart>


<br>
<br>

### 2. Viz for Under 5, 5-14 Children Mortality Rate
<vegachart schema-url="{{ site.baseurl }}/assets/json/map_plots.json" style="width: 100%"></vegachart>

<br>


### 3. To compare GDP and Children under 5 Mortality Rate
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_mortality_map.json" style="width: 100%"></vegachart>

<br>
<div class="left">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/mortality_5.json" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/seoyoung-aspyn/seoyoung-aspyn.github.io/blob/main/python_notebooks/IS445_Final3.ipynb" text="Codes" %}
</div>