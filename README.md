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

This project performs a comprehensive analysis of **sales data from 2019 to 2022**, covering ~88K customers and ~93K transactions. The goal is to evaluate business performance across revenue, orders, product profitability, refunds, loyalty programs, and regional demand and finally deliver **actionable insights** to support cross-functional teams (Sales, Marketing, Operations, Inventory, and Product).

<details>
<summary> <b>Key Stakeholder Questions</b></summary>
E-Galaxy wants to better understand their performance and any growth opportunities.

- How have **revenue**, **number of orders**, and **Average Order Value (AOV)** trended over time?
- Which **products and brands** drive the most revenue, and which have the highest refund rates?
- How effective is the **Loyalty Program**? Should it be expanded or optimized?
- What are the differences in demand across **regions and countries**?
- How efficient is the **delivery process**, and where can operational improvements be made?
- What recommendations can improve **inventory management**, **marketing**, and **customer experience**?
</details>

<details>
<summary> <b>Data & Tech Info</b> </summary>

- **Data Processing & Analysis**: Python, Pandas, NumPy, Excel, SQL
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Dashboard**: Tableau (explored with Power BI desktop as well)

</details>

[**View Tableau Dashboard**](https://public.tableau.com/views/E-Galaxy/ExecutiveSummary?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)


## Executive Summary
### Sales Performance Overview (2019-2022)
This section analyzes sales performance using **revenue, order volume, and average order value (AOV)** to uncover growth drivers, demand shifts, and actionable opportunities.

<details>
<summary> <b>Click for details and figures</b></summary>

>
><table>
><tr>
>	<b>Table 1.</b> Annual Sales Performance Summary showing yearly sales revenue, number of orders, and average order value (AOV), including year-over-year (YoY) growth rates for each metric.
></tr>
><tr align="center";>
>  <img src="images/yearlytable.png" alt="Annual Sales Performnace Table" width="100%">
></tr>
></table>
>

**Table 1** shows sales revenue grew by **165%** with **102% increase in orders from 2019 to 2020**, driven by Covid-19 pandemic related shifts in consumer behavior, including increased e-commerce activity and work from home trends. In **2021**, order volume continued to rise by **6%** but average order value decline that led to **10% drop in revenue** signalling a shift toward lower value purchases. Revenue has steadily declined from **2020 to 2022**. This downward trend has accelerated between **2021 and 2022** with **orders decreasing by 38%, revenue falling by 44%** and **Avg Order Value (AOV) dropping by 9%** highlighting weakening demand and reduced customer engagement.

>
><table>
><tr align="center">
>  <img src="images/revenuetrend.png" alt="Revenue Trends" width="100%">
></tr>
><tr>
>	<b>Fig. 1. </b> Monthly Sales Revenue Trends. The black line represents monthly sales revenue. Bar height shows the number of orders, while color (gold to purple) reflects the strength of AOV ranging from $217 to $320. Annotations higlights the month with the highest Revenue and the month with highest month-over-month growth rate. The grey shaded area highlights 2020 during which the revenue, order volume, and AOV peaked.
></tr>
></table>
>

**Fig. 1** shows monthly revenue and order dynamics where sales revenue peaked in **May 2020** and monthly revenue reached approximately **$1M** reflecting the pandemic driven e-commerce surge. This was accompanied by increased num of orders. **March 2020** showed the highest monthly growth rate of **50%** compared to previous month. The purple bars patch is concentrated between January 2020 and Q1 of 2021 reflecting peak AOV, order volume, and sales revenue.

>
><table>
><tr align="center">
>  <img src="images/customertrend.png" alt="Customer Trends" width="100%">
></tr>
><tr>
>  <b>Fig. 2. </b> Monthly  Customer  Trends by loyalty status. Green represents loyalty members and orange represents non-loyalty customers. The grey shaded area highlights 2020 during which non-Loyalty customers peaked while loyalty membership increased significantly. 
></tr>
></table>
>

**Fig. 2** shows monthly customer trends segmented by loyalty status. Non-Loyalty customers were the primary drivers of growth between 2019 and 2021 with  a sharp surge in non-loyalty customers that peaked in May 2020. 

Since 2020, there is a notable shift to loyalty membership. Loyalty customers have increased significantly throughout 2020, eventually surpassing non-loyalty customers by the end of the year and  peaked in Feb 2021. This indicates successful conversion and retention. Both customer segments have stabilized in 2021 suggesting a plateau in customer expansion and engagement. However, beginning in April 2022, both loyalty and non-loyalty customers count  have sharply declined mirroring drop in orders and revenue (Fig. 1). This implies a contraction in the whole customer base rather than an isolated segment issue.
</details>

**Key Insights**
- **Pandemic driven surge in 2020** with increased revenue (**~165%**) primarily driven by a **~102% increase in order volume**, indicating demand expansion rather than pricing power.
- **Revenue is volume driven**  as changes in revenue closely track order volume, while AOV remains relatively stable within a narrow band of **$217-$320**.
- **Post-peak normalization** as demand patterns indicate a reversion following pandemic-driven boom.
- **Demand contraction in 20222** with declined Revenue (-44%), Orders (-38%), AOV (-9%) signaling deeper demand challenges.
- **Customer shifted from non-loyalty to loyalty memberships** post 2020. But 2022 showed decline across both segments indicating systemic demand issues.
- **Further deep analysis required**

**Business Implications**
- Growth during 2020 was **externally driven (pandemic effects)** and not structurally sustainable.
- 2022 decline suggests **customer acquisition and retention breakdown**.
- The business lacks **strong AOV expansion mechanisms**.

**Recommendations**
- **Increase AOV** through product bundling, upselling, and pricing optimization strategies.
- **Rebuild Customer demand** by strenghtening customer acquisition and retention program by relaunching loyalty program incentives and targeted campaigns.
- **Analyze behaviour of loyalty members** to identify opportunities for increasing purchase frequency and lifetime value
- **Reassess customer behaviour** by analyzing post-pandemic shifts to realign product offerings and marketing strategy for sustainable consumption patterns.


## Deeper Insights
### Product Performance Analysis
This section analyzes product level performance using monthly revenue trends, product contribution (Pareto analysis), and order volume vs revenue segmentation. The goal is to identify **high impact products**, **uncover inefficiencies**, and **provide data driven recommendations**.

<details>
<summary> <b>Click for details and figures</b></summary>

>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/producttrend.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/productpareto.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 3a.</b> Monthly revenue trends segmented by product. <b>3b.</b> Product Contribution and Segmentation Analysis. <b>Top row:</b> Pareto analysis of product revenue contribution. The grey reference line represents the 80% cumulative revenue threshold. <b> Bottom row:</b> Product segmentation to four quadrants based on median revenue (horizontal grey lines) and median order volume (vertical grey lines)
></td></tr>
> </table>
>

**Fig. 3a.** shows the monthly revenue trends by product. Among the eight products, **27in 4k Gaming Monitor, Apple Airpods**, and **MacBook Air**  are the top products consistently driving the majority of revenue from 2019 to 2022. The Parteo Analysis (**Fig. 3b., top row**) shows that these three products contribute **~85%** of the total revenue. Additionaly, the **Thinkpad laptop** accounts for a further **~11%**, bringing combined contribution of top four products to **~86%** of total revenue. All four products experienced a significant peak during the the pandemic driven market in 2020 followed by gradual normalization from 2021 to 2022, reflecting declining demand. 

**Fig. 3b [bottom row]** presents product segmentation analysis based on median revenue and order volume, dividing products into four quadrants.
| Segment          | Characteristics                  | Products                                      |
|------------------|----------------------------------|-----------------------------------------------|
| **Star**         | High revenue + High volume (HH)      | Apple AirPods, 27in 4K Gaming Monitor     |
| **Volume Drivers** | Low revenue + High volume (LH)      | Samsung accessories (charging cables, webcams) |
| **Premium**      | High revenue + Low volume (HL)       | MacBook Air Laptop, ThinkPad Laptop          | 
| **Underperformers** | Low revenue + Low volume (LL)     | Apple iPhone, Bose SoundPort                 |

 The scatter plot shows that **Apple Airpods** are the highest selling product, followed by **27in 4k Gaming Monitor**. Both are firmly positioned in the **High revenue, High volume (HH)** quadrant, making them the company's **Star products**. 

 **Samsung accessories** (charging cables and webcams) fall into the **Volume drivers** category that generates high order volume but relatively low revenue per order.

**Premium products** includes **MacBook Air and ThinkPad laptops** that generates high revenue but have lower sales volume. Notably, the MacBook Air is  positioned close to the **Star quadrant**. This implies potetntial for growth. However, both premium products have **high refund rate **(>11%)** which is a significant concern.

**Undepreforming products** such as **Apple iPhone and Bose headphones** show low revenue and low order volume. Despite this, the iPhone has a **high AOV (~$743)** but still suffers from a relatively high **refund rate(~8%)** suggesting customer dissatisfcation.
</details>

<details>
  <summary> <b>Key Insights and Recommendations for Product Team</b> </summary>
 **Key Insights**
- Revenue is primarily driven by top three products. They contribute 85% of total revenue indicating heavy reliance on a limited product.
- **Product Segmentation**
| Segment          | Products         | Action                             |
|------------------|----------------------------------|-----------------------------------------------|
| **Star**         | Apple AirPods, 27in 4K Gaming Monitor     | Scale marketing, enusre inventory |
| **Volume Drivers** | Samsung accessories (charging cables, webcams) | Bundle to increase AOV|
| **Premium**      | MacBook Air Laptop, ThinkPad Laptop (Higher refund rate)          | Investigate and reduce refund issues |
| **Underperformers** | Apple iPhone, Bose SoundPort | Reposition or consider phase out|      

- **Critical issues identified**
  - **High refund rates (>11%)** in premium product **laptops**. Possible causes might be product expectation mismatch, quality issues, or logistics problems.
  - **Underperforming Applie iPhone** have high AOV but low demands. Refund rates are also relatively high (**~8%**) indicating potential positioning or pricing issues. 
  - **Missing refund data for 2022** . This represents **data quality issues** limting accurate performance evaluation, refund trend analysis and inventory planning.

 **Recommendations**
- Priortitize on star products with targeted marketing, promotions, and inventory optimization as they are the primary revenue drivers.
- Fix refund problem (**High Priority**) on premium products by conducting root cause analysis by reviewing return reasons, customer feedback, delivery issues and others.  Reducing refund rates will have a **direct positive impact on profitability.**
- Monetize volume drivers by bundling accessories with high value products (e.g. monitors, laptops) to increase AOV.
- Reassess Bose soundport and iPhone and decide on whether to improve their positioning and marketing  or phase out if performance does not improve.
- Resolve data gaps by further investigation on missing refund data for 2022 as it limits visibility into product performance, refund analysis, inventory planning, and forecasting.
</details>

### Customer, Geographic, Marketing, and Operational
<details>
<summary> <b>Click for details and figures (in Progress)</b></summary>

### Customer Performance by Loyalty Membershipb

>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/customersrevenue.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/customerorderdist.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 4a.</b>  <b>4b.</b> 
></td></tr>
> </table>
>


### Geographic Performance

>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/countryperformance.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/countrypareto.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 5a.</b>  <b>5b.</b> 
></td> </tr>t
> </table>
>


>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/regionperformance.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/regionrefundrate.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 6a.</b>  <b>6b.</b> 
></td></tr>
> </table>
>



### Marketing Channel Performance

>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/marketingchannelperformance.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/marketingchannelrefundrate.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 8a.</b>  <b>8b.</b> 
></td></tr>
> </table>
>



### Operational Performance

>
> <table width="100%">
>   <tr>
>     <td align="center" width="50%">
>       <img src="images/deliverytimetrend.png" width="100%"><br>
>     </td>
>     <td align="center" width="50%">
>       <img src="images/deliverytimedist.png" width="100%"><br>
>     </td>
>   </tr>
>   <tr>
>     <td colspan="2">
>       <b>Fig. 9a.</b>  <b>9b.</b> 
></td></tr>
> </table>
>

</details>
