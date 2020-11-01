# Tableau - Citi Bike Analytics

[Link to Tableau Public Profile](https://public.tableau.com/profile/david.fried8413#!/)

## Overview

Ioana Hancu from the Monday/Wednesday class and I collaborated on this assignment.

We gathered bike data from Summer 2019 and Summer 2020 Citi Bike Trip History Logs, and analyzed the data with Tableau. Several visualizations, two dashboards, and a Story were produced with Tableau Public.

##### Data Munging

Prior to analysis with Tableau, we used Pandas in Jupyter Lab (combined_data.ipynb) to create one big CSV from eight CSV files of bike data:

* JC-201906-citibike-tripdata.csv
* JC-201907-citibike-tripdata.csv
* JC-201908-citibike-tripdata.csv
* JC-201909-citibike-tripdata.csv
* JC-202006-citibike-tripdata.csv
* JC-202007-citibike-tripdata.csv
* JC-202008-citibike-tripdata.csv
* JC-202009-citibike-tripdata.csv

##### Outliers

We used Tableau to deal with outliers by using filters to exclude bad data in visualizations (e.g., individuals who claim they were 130 years old).

##### The Impact of COVID-19 Story

This story contains several visualizations comparing bike statistics between Summer 2019 (June, July, August, and September) and Summer 2020 (June, July, August, and September). The first visualization (Number of Bike Rides) shows a greater number of rides in Summer 2019 compared with summer 2020, which may be attibutable to individuals staying inside to avoid COVID-19. Interestingly, the second visualization (Bike Inventory) shows more bikes available during Summer 2020. I speculated that more bikes may have been purchased in 2020 because the bike company anticipated that the pandemic would result in more people using bikes to avoid crowded spaces on public transportation. Data from October 2020 were included in the original September 2020 CSV file. A filter was used on both visualizations to remove 2020 October data so the analysis between summers was consistent in months.

The third visualization from the story (Popularity of Stations over Time) shows changes in the popularity of bike stations between the two summers. The distribution of bike rides was more spread out in Summer 2020, perhaps due to less concentrations of people in the heart of the City. The map is interactive in that it displays changes in station popularity each time a summer month is clicked. Zip codes are overlaid on top.

The final visualization of the story (Busiest Times) shows the busiest times for each summer. It was noted that people were less likely to ride bikes during the morning in Summer 2020 compared with Summer 2019. However, in Summer 2020 individuals were much more likely to ride bikes during the weekend. Perhaps less people were commuting to work on bikes during the weekdays in 2020 because they were working from home as a result of the pandemic.

##### Other Visualizations

Visualizations not included in the above story were Age Distribution and Trip Duration. For the Age Distribution visualization, several individuals reported erroneous ages (e.g., 130 years old). We categorized age in bins of five years and excluded anyone over 90 years old. The visualization shows that the 30 to 35 year-old age category had the highest percentage of rides. The Trip Duration visualization is a map of the average duration of bike rides for each station.