# E-Galaxy Sales Performance Analysis

#### End-to-End Data Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)](https://www.python.org)
[![Tableau Public](https://img.shields.io/badge/Tableau%20Public-E97627?logo=tableau&logoColor=white)](https://public.tableau.com)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<p align="center">
  <img src="images/companylogo.png" alt="E-Galaxy Logo" width="200" height="200">
</p> 

**E-Galaxy** is a global e-commerce company specializing in electronics products like laptops, smartphones, headphones, and accessories from leading brands like **Apple**, **Samsung**, **Lenovo**, and **Bose**. Founded in 2018, the company operates through web and mobile platforms.

This project performs a comprehensive analysis of **sales data from 2019 to 2022**, covering ~88K customers and ~93K transactions. The goal is to evaluate business performance across revenue, orders, product profitability, refunds, loyalty programs, and regional demand, then deliver **actionable insights** to support cross-functional teams (Sales, Marketing, Operations, Inventory, and Product).

<details>
<summary> Data & Tech Info </summary>

**Tech Stack**: Python, Pandas, NumPy, Matplotlib, Seaborn, Tableau, Excel

</details>

<details>
<summary>Key Stakeholder Questions</summary>
E-Galaxy wants to better understand their performance and any growth opportunities.

- How have **revenue**, **number of orders**, and **Average Order Value (AOV)** trended over time?
- Which **products and brands** drive the most revenue, and which have the highest refund rates?
- How effective is the **Loyalty Program**? Should it be expanded or optimized?
- What are the differences in demand across **regions and countries**?
- How efficient is the **delivery process**, and where can operational improvements be made?
- What recommendations can improve **inventory management**, **marketing ROI**, and **customer experience**?
</details>

<details>
<summary> Data & Tech Info </summary>

- **Data Processing & Analysis**: Python, Pandas, NumPy, Excel
- **Visualization**: Matplotlib, Seaborn
- **Dashboard**: Tableau (primary) + Power BI (exploratory)

</details>


[**View Tableau Dashboard**](https://public.tableau.com/views/E-Galaxy/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)


## Executive Summary
### Sales Performance Overview (2019-2022)
<p style="text-align: justify;">
	<b>Table 1.</b> Annual Sales Performance Summary showing yearly sales revenue, number of orders, and average order value (AOV), including year-over-year (YoY) growth rates for each metric.
</p>
<p align="center";>
  <img src="images/yearlytable.png" alt="Annual Sales Performnace Table" width="600" height="1200">
</p> 

**Table 1** shows sales revenue grew by **165%** with **102% increase in orders from 2019 to 2020**, driven by Covid-19 pandemic related shifts in consumer behavior, including increased e-commerce activity and work from home trends. In **2021**, order volume continued to rise by **6%** but average order value decline that led to **10% drop in revenue** signalling a shift toward lower value purchases. Revenue has steadily declined from **2020 to 2022**. This downward trend has accelerated between **2021 and 2022** with **orders decreasing by 38%, revenue falling by 44%** and **AOV dropping by 9%** highlighting weakening demand and reduced customer engagement.

<p align="center">
  <img src="images/RevenueTrends.png" alt="Revenue Trends" width="800" height="600">
</p>

<p style="text-align: justify;">
	<b>Fig. 1. </b> Monthly Sales Revenue Trends. The black line represents monthly sales revenue. Bar height shows the number of orders, while color (gold to purple) reflects the strength of AOV ranging from $217 to $320. Annotations higlights the month with the highest Revenue and the month with highest month-over-month growth rate.
</p>

**Fig. 1** shows sales revenue peaked in **May 2020** and monthly revenue reached approximately **$1M** reflecting the pandemic driven e-commerce surge. This was accompanied by increased num of orders. **March 2020** showed the highest monthly growth rate of **50%** compared to previous month. The purple bars patch is concentrated between January 2020 and Q1 of 2021 reflecting peak AOV, order volume, and sales revenue.

**Key Insights**
- **Revenue is primarily volume driven**. Changes in revenue closely tracks changes in order volume rather than AOV.
- **AOV remained relatively stable** within a narrow band of **$217-$320** contributing minimally to revenue volatility.
- **Structural demand decline**. The sharp drop in 2022 orders suggests challenges in **customer acquisition, retention, or purchase frequency**, not pricing.
- **Post-peak normalization** Demand patterns indicate a reversion following pandemic-driven boom.
- **Further deep analysis required**

**Recommendations**
- **Boost AOV** through bundling, upselling, and pricing optimization strategies
- **Rebuild demand** by strenghtening customer acquisition and retention initiatives
- **Reassess customer behaviour** by analyzing post-pandemic shifts to realign product and marketing strategy
- **Deep-dive analysis** by segemnting customers and channels to identify specific drivers of decline
