---
name: Final Project 3
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization.png
description: This is the assignment 10 from group 22
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Fianl_Project_3

### Group 6

Zhizhou Xu, Yeting Qi, Jindi Zhang

<vegachart schema-url="{{ site.baseurl }}/assets/json/PPG_AGE.json" style="width: 100%"></vegachart>
This visualization shows the distribution of temperature from 50 states of the US. X axis is the highest temerature record and the y axis are the states. The color from light green to dark blue in every block means the number of records in that specific range of temperature. As you can see, we used "rect" mark to visualize this dataset because we wanted to make it as a heatmap. We also chose "orangered" as our color scheme because by using this color scheme, we can feel a sense of heat.

<vegachart schema-url="{{ site.baseurl }}/assets/json/PPG_position.json" style="width: 100%"></vegachart>
In this visualization, we used bar chart to show the highest temerature distribution throughout the country. We chose bar chart because a bar chart can make a good demonstration on how many records in different range of temperature respectively. We also chose orange to render the bar chart. Additionally, we added a simple interaction to this bar chart. When users hover their mouse on a bar in this chart, it will show the detail of this bar. In this case, it will show the highest temperature and the frequency.

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_temperature.json" style="width: 100%"></vegachart>
We also followed the instructions from week 11 class and linked these two visualizations. We added brush selection to the heatmap on the left to select the sector that we wanted to show in the histogram on the right. The interactions worked OK but the tooltip in the histogram seemed not working. If we had more time, we would want to fix this issue and explore more interactions in vega lite and altair.

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/DaBaLxx/DaBaLxx.github.io/blob/main/python_notebooks/group-22-assignment-10.ipynb" text="The Analysis" %}
</div>
