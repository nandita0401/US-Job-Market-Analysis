This project analyzes the relationship between US population growth and unemployment trends from 2020 to 2023 using Tableau and Python. The goal is to explore whether an increasing population influences unemployment rates.


**Problem Statement**: The US population has been steadily increasing over the years, raising important questions about its impact on the job market. A growing population could mean a larger workforce, potentially driving economic growth and job creation, but it could also lead to increased competition for available jobs, influencing unemployment rates. This project aims to analyze the relationship between population growth and unemployment trends from 2020 to 2023 using data from the Bureau of Labor Statistics and US Census. By examining these trends through data visualization in Tableau, we seek to determine whether population growth directly affects unemployment or if other external factors, such as economic policies or global events like COVID-19, play a more significant role in shaping employment patterns.


**Datasets Used**

This analysis uses two key datasets:
1️⃣ **BLS Unemployment Data (2020-2023)** – Provides yearly unemployment rates.
2️⃣ **US Population Data (2020-2023)** – Contains population estimates for the same period.
The datasets were cleaned using Python and prepared in Tableau for visualization.

**Data Cleaning & Preparation**: The raw population dataset had separate columns for each year, which were reformatted into a structured table. The unemployment dataset contained monthly data, which was aggregated into yearly averages. This ensured that both datasets could be joined on Year in Tableau.


**Visualizations in Tableau & Insights**

1️⃣ **Population vs. Unemployment (Dual-Axis Chart) – Top Left**
This graph compares population (blue) and unemployment rate (red) over time.
Insight: While the population has increased, unemployment fluctuated, indicating that population growth alone does not directly cause changes in unemployment.


2️⃣ **US Population Growth (Line Chart) – Top Right**
This shows the steady increase in the US population from 2020-2023.
Insight: The population growth rate appears stable, reinforcing the idea that the labor force is expanding yearly.


3️⃣ **Unemployment Rate Over Time (Bubble Chart) – Bottom Left**
This represents unemployment rate trends across years.
Insight: 2020 had the highest unemployment rate, likely due to COVID-19, but it decreased in subsequent years.

4️⃣ **Correlation: Population vs. Unemployment (Scatter Plot) – Bottom Right**
This examines whether a larger population leads to higher or lower unemployment.
Insight: The scatter plot does not show a strong upward or downward trend, indicating no strong correlation between population size and unemployment rate.

**Key Findings**: Population is rising, but unemployment does not follow a clear trend, suggesting other factors influence job availability.
2020 had the highest unemployment rate, likely due to external factors (COVID-19), rather than population changes.
The relationship between population growth and unemployment is weak, meaning economic policies, job market demand, and global events likely play a bigger role in unemployment trends.

**Next Steps & Future Analysis**: Including industry-specific employment trends to see which sectors were most affected.
Adding wage growth and inflation data to analyze broader economic trends.
Forecasting future unemployment trends based on historical data.

**Conclusion**: This project highlights how data visualization and analysis can uncover key economic trends. By leveraging Python for data cleaning and Tableau for interactive insights, we gain a clearer understanding of how population and unemployment interact over time.

Would love to hear feedback or suggestions for further improvements!
