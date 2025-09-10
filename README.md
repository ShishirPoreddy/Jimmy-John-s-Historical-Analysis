# Jimmy John’s Economic Data Analysis  


## Overview  
This project investigates **seasonal and holiday demand fluctuations** in foot traffic at Jimmy John’s locations using SafeGraph visit data from **2018–2022**. The analysis explores how **average daily visits** change across seasons, with a particular focus on the significant decline in visits during **winter months (December–January)** compared to peak summer months.  

By applying statistical analysis and data visualization, this project provides actionable insights into how **staffing, inventory, and marketing strategies** could be adjusted to maximize profits during high-demand periods and minimize losses during low-demand periods.  

---

## Objectives  
1. **Seasonal Trends** – Test whether summer months (June–September) show significantly higher average daily visits compared to winter months (December–February).  
2. **Holiday Transition Analysis** – Identify whether the largest percentage decrease in visits occurs between **November → December** and test its statistical significance.  
3. **Operational Implications** – Translate findings into recommendations for **staff scheduling, inventory control, and marketing adjustments**.  

---

## Methodology  

- **Data Source**: SafeGraph foot traffic data (`jj_long` dataset).  
- **Variables**:  
  - Dependent: Average daily visits  
  - Independent: Month/Season, Transition Period  
  - Controls: Year, Region, Day of Week, Holiday Indicators  
- **Statistical Tests**:  
  - Two-sample t-test for seasonal differences (Summer vs Winter).  
  - Paired t-test for pre-winter vs winter transition (Oct–Nov vs Dec–Jan).  
- **Visualization & Tools**:  
  - `pandas` – Data cleaning and aggregation  
  - `numpy` – Calculations (e.g., percentage change)  
  - `scipy.stats` – Statistical testing  
  - `matplotlib` – Visualizations (line graphs, bar charts)  
  - `datetime` – Date handling  

---

## Key Findings  

- **Seasonal Effect**:  
  Jimmy John’s visits consistently peak in summer (June–September) and decline in winter (December–February) across all years except when impacted by COVID-19 or major corporate events (e.g., Inspire Brands acquisition in 2019).  

- **Holiday Transition Drop**:  
  The largest **statistically significant percentage decline** occurs between **November → December**, with visits dropping by over **60% in some years**.  

- **Business Implications**:  
  - **Staffing**: Reduce staff during low-demand winter months; increase coverage during summer.  
  - **Inventory**: Adjust purchasing to prevent food waste during drought months.  
  - **Marketing**: Boost promotions and campaigns in winter to offset reduced foot traffic.  

---

## Project Structure  

- **ECON433-proj1-ShishirPoreddy-JimmyJohns.ipynb** – Introductory analysis  
- **ECON433-proj2-ShishirPoreddy-JimmyJohn's.ipynb** – Seasonal trends analysis  
- **ECON433-proj3-ShishirPoreddy-JimmyJohns.ipynb** – Transition period analysis  
- **ECON433-proj4-ShishirPoreddy-JimmyJohn's.ipynb** – Final models & visualizations  
- **annotated-Poreddy_Individual_Final_Report.pdf** – Final written report  
- **README.md** – Project documentation  
