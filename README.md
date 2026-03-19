# 📊 US Job Market Analysis — Population vs. Unemployment Trends

![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Tableau](https://img.shields.io/badge/Visualization-Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![Jupyter](https://img.shields.io/badge/Tool-Jupyter%20Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Data Source](https://img.shields.io/badge/Data-BLS%20%7C%20US%20Census-4285F4?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

> A data analysis and visualization project examining the relationship between US population growth and unemployment trends from 2020 to 2023 — using Python for data cleaning and Tableau for interactive visual insights drawn from Bureau of Labor Statistics and US Census data.

---

## 📖 Table of Contents

- [About the Project](#about-the-project)
- [Problem Statement](#problem-statement)
- [Datasets](#datasets)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Visualizations & Insights](#visualizations--insights)
- [Key Findings](#key-findings)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

## About the Project

Does a growing population drive unemployment up — or does economic expansion absorb new workers? This project investigates that question using real government data from the **Bureau of Labor Statistics (BLS)** and the **US Census Bureau**, covering the period from 2020 to 2023 — a timeframe that includes one of the most dramatic labor market disruptions in modern history: the COVID-19 pandemic.

By combining **Python-based data preprocessing** with **Tableau dashboards**, this project demonstrates a full data analytics workflow from raw government datasets to actionable visual insights.

---

## Problem Statement

> *The US population has been steadily increasing, raising important questions about its impact on the job market. A growing population could mean a larger workforce and economic growth — but it could also intensify competition for available jobs. This project analyzes whether population growth directly affects unemployment rates, or whether external factors like COVID-19 and economic policy play a more significant role.*

---

## Datasets

| Dataset | Source | Description |
|---|---|---|
| `BLS_Unemployment.csv` | Bureau of Labor Statistics | Yearly US unemployment rates (2020–2023) |
| `Cleaned_Population_USA.csv` | US Census Bureau | US population estimates (2020–2023) |

Both datasets were joined on **Year** in Tableau after preprocessing in Python.

---

## Data Cleaning & Preparation

Performed in Python (`dataset.ipynb`):

- **Population dataset** — Reformatted from wide format (separate columns per year) into a structured long-format table suitable for Tableau joins
- **Unemployment dataset** — Removed unrelated records and standardized column formats
- Both datasets aligned on a common `Year` key to enable cross-dataset analysis in Tableau

---

## Visualizations & Insights

Four Tableau visualizations were built to explore the data from different angles:

**1. Population vs. Unemployment — Dual-Axis Chart**
Plots population (blue) and unemployment rate (red) on the same timeline.
**Insight:** Despite rising population, unemployment fluctuated independently — suggesting population growth alone does not drive unemployment changes.

**2. US Population Growth — Line Chart**
Tracks steady population increase from 2020 to 2023.
**Insight:** The growth rate is stable year-over-year, confirming a consistently expanding labor force.

**3. Unemployment Rate Over Time — Bubble Chart**
Visualizes unemployment trends with bubble size representing magnitude.
**Insight:** 2020 shows a dramatically larger bubble — the COVID-19 spike — which normalized in subsequent years.

**4. Population vs. Unemployment Correlation — Scatter Plot**
Examines whether larger population correlates with higher or lower unemployment.
**Insight:** No strong upward or downward trend observed — confirming a **weak correlation** between population size and unemployment rate.

---

## Key Findings

- 📈 **Population is rising** but unemployment does not follow a proportional trend — other factors dominate
- 😷 **2020 had the highest unemployment rate** — attributable to COVID-19 rather than population dynamics
- 🔗 **Weak correlation** between population growth and unemployment — economic policy, global events, and industry demand are stronger drivers
- 📉 **Unemployment declined consistently** from 2021–2023 as the economy recovered, independent of population changes

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Data cleaning and preprocessing |
| Pandas | Dataset restructuring and formatting |
| Jupyter Notebook | Interactive data preparation environment |
| Tableau | Interactive dashboard and visualization |
| BLS & US Census Data | Primary government data sources |

---

## Getting Started

### Prerequisites
```bash
pip install pandas numpy jupyter
```

Tableau Desktop or Tableau Public is required to open the `.twb` file.

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/nandita0401/US-Job-Market-Analysis.git
   cd US-Job-Market-Analysis
```

2. **Run the data preparation notebook**
```bash
   jupyter notebook dataset.ipynb
```

3. **Open the Tableau workbook**
```
   Open Unemployment.twb in Tableau Desktop or Tableau Public
   Connect to BLS_Unemployment.csv and Cleaned_Population_USA.csv when prompted
```

---

## Project Structure
```
US-Job-Market-Analysis/
├── dataset.ipynb                  # Python data cleaning notebook
├── BLS_Unemployment.csv           # Bureau of Labor Statistics unemployment data
├── Cleaned_Population_USA.csv     # US Census population data (cleaned)
├── Unemployment.twb               # Tableau workbook with all 4 dashboards
└── README.md
```

---

## Future Improvements

- [ ] Add **industry-specific employment trends** to identify sectors most impacted by population and economic shifts
- [ ] Incorporate **wage growth and inflation data** for a broader macroeconomic picture
- [ ] Build **unemployment forecasting model** using time series analysis (ARIMA / Prophet)
- [ ] Expand dataset to **2015–2024** for longer trend visibility
- [ ] Publish interactive dashboard to **Tableau Public** for live access
- [ ] Add **state-level breakdown** to surface regional unemployment disparities

---

## Author

**Nandita Bharambe**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-nanditabharambe-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/nanditabharambe/)
[![GitHub](https://img.shields.io/badge/GitHub-nandita0401-181717?style=flat&logo=github)](https://github.com/nandita0401)

---

> 💡 *This project reinforced that data rarely tells a simple story. The instinct to assume population growth drives unemployment is intuitive — but the data shows that external shocks like COVID-19 and policy responses are far more powerful forces. Good analysis challenges assumptions.*
