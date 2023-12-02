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

## Contextualizing Child Mortality Rates Around the World
By Seoyoung Yoon, Nicole Gromski, Sahithi Manne (Group 13)
<br>
<br>
<br>

In the grand scheme of global health, we're diving deep into the heart-wrenching tale of child mortality rates-those crucial numbers that show how well societies are able to take care of the youngest members of their communities.<br> 

Picture this: 1800, a time when saying goodbye to more than a third of kids before their fifth birthday was, unfortunately, par for the course. Fast forward to 1950, and things start looking up-but not for everyone.<br>  Now, move to 2022, and the data visualizations we show here become the superheroes in our story, showing off the incredible progress we've made as a global society. 


<br> 
<br>
<br>

## Global View: Under-5 Mortality Rate Insights Dashboard
Click on any country on the map to see a line chart illustrating its child mortality trends over the years!
<br> 
<vegachart schema-url="{{ site.baseurl }}/assets/json/new_chart.json" style="width: 100%"></vegachart>
Child under 5 mortality rate dataset is from worldbank.org &nbsp; ➭  &nbsp;  {% include elements/button.html link= "https://data.worldbank.org/indicator/SH.DYN.MORT" text="Link" %}

<div id="vis"></div>

<br>

We can see from the above visualization how the child mortality rates look around the world right now. <br> 
The majority of the countries around the world are highlighted in green because their mortality rates are low, but unfortunately, there are still many countries highlighted in darker blue shades.<br> These countries are the ones with the highest child mortality rates around the world. If we click on any of these countries, even the ones with the highest mortality rates, we can see how their child mortality rate has decreased in the last few decades, even if it is at a slow pace for some countries. <br> This progress is great to see, and it is important because it shows how global initiatives have helped, and we need to continue to support them. 

<br> 
<br>
<br> 
<br>
<br> 

## ☑️ Contextualizing these Child Mortality Rates
<br>

### Child Mortality Rates in 2022: Under 5 vs. 5 to 14 Years
<vegachart schema-url="{{ site.baseurl }}/assets/json/map_plots.json" style="width: 100%"></vegachart>
Child aged 5-14 mortality rate dataset is from childmortality.org &nbsp; ➭  &nbsp;  {% include elements/button.html link= "https://childmortality.org/" text="Link" %}
<br> 
<br>

Our visualization provides a comparative view of child mortality rates for two distinct age groups: under 5 and from 5 to 14 years old, as recorded in 2022. Through two adjacent interactive maps, viewers can hover over countries to reveal a tooltip with the latest mortality figures, offering a clear and immediate comparison between the vulnerabilities of these age groups. This visualization highlights not only the disparities in child health across different regions but also serves as a vital tool for understanding where improvements have been made and where challenges persist. By presenting these two age brackets side by side, we aim to bring to light the progress in global health initiatives and the areas that require continued focus and action.
<br> 
<br>
<br>
<br> 
<br>
<br>
<img src="https://ourworldindata.org/images/published/3-maps-of-Child-mortality_850.webp" alt="Children mortality in 1800, 1950, and 2015">
This image is from ourworldindata.org &nbsp; ➭  &nbsp;  {% include elements/button.html link= "https://ourworldindata.org/child-mortality-global-overview" text="Link" %}
<br> 
<br>
We could see from the previous visualizations how child mortality had improved from 1960 to the current time, but we can see the drastic difference from the last two centuries in this visualization. In 1800, more than one-third of children worldwide did not survive to age five, making child deaths a common occurrence. By 1950, advancements in living standards, healthcare, and nutrition had significantly reduced child mortality in affluent regions, but it remained high in other parts of the world. We can see how in 1800, the entire world was in red, which meant very high mortality rates, while in 1950, there was only red in some developing nations. <br>
Fast-forwarding to 2015, global progress is evident, with substantial declines in child mortality rates across all regions. We can see how no countries have a mortality rate of above 20% as shown by the lack of countries highlighted in orange or red on the 2015 map. We can see from the child mortality in 2015 visualization, along with other visualizations on this page, that despite progress, the frequency of child deaths remains tragically high in some areas. This data really highlights the ongoing importance of global initiatives to improve child survival rates. 


<br> 
<br>
<br>
<br> 
<br>
<br>

### GDP effects and population size on Child Mortality Rates
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_map.json" style="width: 100%"></vegachart>
GDP dataset is from worldbank.org &nbsp; ➭  &nbsp;  {% include elements/button.html link= "https://data.worldbank.org/indicator/NY.GDP.MKTP.CD" text="Link" %}
<br> 
<br>
This world map provides a visual overview of the global income landscape, categorized by countries’ Gross Domestic Product (GDP). The GDP is the measure of the monetary value of a country’s goods it produces which correlates to whether a country is a higher, middle, or lower-income nation. This attributes to a nation’s and its people’s access to proper vital resources such as food, water, and healthcare. A lack of these resources and economic prosperity has been seen to influence a country’s rate of medical advancements as well. The map is color-coded to differentiate between high, upper-middle, lower-middle, and low-income nations. With intuitive color distinctions, viewers can discern the economic tiers of each country. Hovering over a nation reveals a tooltip with its income group, offering an instant snapshot of its economic status. This graph can be used as supplementary data when combined with the child mortality rates world map to identify possible trends in a nation’s income levels and their child mortality rates.

<br>
<br> 
<br>
<br> 
<br>
<br>

### Economic Profiles vs. Child Health
A Comparative Analysis of GDP and Under-5 Mortality
<vegachart schema-url="{{ site.baseurl }}/assets/json/gdp_mortality_map.json" style="width: 100%"></vegachart>
<br> 
<br>
This visualization presents a comparative analysis of GDP income groups and under-5 mortality rates in 2022, illustrating the intersection of economic status and child health outcomes. The map on the left shows the world's nations categorized by income level: high, upper-middle, lower-middle, and low, with a specific color assigned to each category. The map on the right details the under-5 mortality rates, with color intensity indicating the severity, ranging from lower rates in green to higher rates in blue. The visual data suggest that lower-income countries tend to have higher child mortality rates, while high-income countries show lower rates, highlighting the impact of economic conditions on child health. The stark contrast across continents, especially visible in African countries with both low GDP and high child mortality rates, underscores the global inequalities in health and economic prosperity.
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