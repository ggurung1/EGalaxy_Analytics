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

This project performs a comprehensive analysis of **sales data from 2019 to 2022**, covering ~88K customers and ~93K transactions. The goal is to evaluate business performance across revenue, orders, product profitability, refunds, loyalty programs, and regional demand and finally deliver **actionable insights** to support cross-functional teams (Sales, Product, Cusatomer, Marketing, Operations, and Inventory).

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
>	<b>Fig. 1. </b> Monthly Sales Revenue Trends. The black line represents monthly sales revenue. Bar height shows the number of orders, while color (gold to purple) reflects the strength of AOV ranging from $217 to $320. Annotations higlights the month with the highest revenue and the month with highest month-over-month growth rate. The grey shaded area highlights 2020 during which the revenue, order volume, and AOV peaked.
></tr>
></table>
>

**Fig. 1** shows monthly revenue and order dynamics where sales revenue peaked in **May 2020** and monthly revenue reached approximately **$1M** reflecting the pandemic driven e-commerce surge. This was accompanied by increased number of orders. **March 2020** showed the highest monthly growth rate of **50%** compared to previous month. The purple bars patch is concentrated between January 2020 and Q1 of 2021 reflecting peak AOV, order volume, and sales revenue.

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
- **Demand contraction in 2022** with declined Revenue (-44%), Orders (-38%), AOV (-9%) signaling deeper demand challenges.
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
### 1. Product Performance Analysis

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

**Fig. 3a.** shows the monthly revenue trends by product. Among the eight products, **27in 4k Gaming Monitor, Apple Airpods**, and **MacBook Air**  are the top products consistently driving the majority of revenue from 2019 to 2022. The Parteo Analysis (**Fig. 3b., top row**) shows that these three products contribute **~85%** of the total revenue. Additionaly, the **Thinkpad laptop** accounts for a further **~11%**, bringing combined contribution of top four products to **~96%** of total revenue. All four products experienced a significant peak during the the pandemic driven market in 2020 followed by gradual normalization from 2021 to 2022, reflecting declining demand. 

**Fig. 3b (bottom row)** presents product segmentation analysis based on median revenue and order volume, dividing products into four quadrants.
| Segment          | Characteristics                  | Products                                      |
|------------------|----------------------------------|-----------------------------------------------|
| **Star**         | High revenue + High volume (HH)      | Apple AirPods, 27in 4K Gaming Monitor     |
| **Volume Drivers** | Low revenue + High volume (LH)      | Samsung accessories (charging cables, webcams) |
| **Premium**      | High revenue + Low volume (HL)       | MacBook Air Laptop, ThinkPad Laptop          | 
| **Underperformers** | Low revenue + Low volume (LL)     | Apple iPhone, Bose SoundPort                 |

 The scatter plot shows that **Apple Airpods** are the highest selling product, followed by **27in 4k Gaming Monitor**. Both are firmly positioned in the **High revenue, High volume (HH)** quadrant, making them the company's **Star products**. 

 **Samsung accessories** (charging cables and webcams) fall into the **Volume drivers** category that generates high order volume but relatively low revenue per order.

**Premium products** includes **MacBook Air and ThinkPad laptops** that generates high revenue but have lower sales volume. Notably, the MacBook Air is  positioned close to the **Star quadrant**. This implies potetntial for growth. However, both premium products have **high refund rate (>11%)** which is a significant concern.

**Undepreforming products** such as **Apple iPhone and Bose headphones** show low revenue and low order volume. IPhone has a **high AOV (~$743)** but low demands and suffers from a relatively high **refund rate(~8%)** suggesting customer dissatisfcation.
</details>

<details>
  <summary> <b>Key Insights and Recommendations</b> </summary>

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
- **Fix refund problem** (<font color="red"><b>High Priority</b></font>) on premium products by conducting root cause analysis by reviewing return reasons, customer feedback, delivery issues and others.  Reducing refund rates will have a **direct positive impact on profitability.**
- Monetize volume drivers by bundling accessories with high value products (e.g. monitors, laptops) to increase AOV.
- **Reassess Bose soundport and iPhone** and decide on whether to improve their positioning and marketing  or phase out if performance does not improve.
- **Resolve data gaps** by further investigation on missing refund data for 2022 as it limits visibility into product performance, refund analysis, inventory planning, and forecasting.
</details>


### 2. Customer Performance by Loyalty Membership

<details>
<summary> <b>Click for details and figures</b></summary>

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
>       <b>Fig. 4a.</b> Customer revenue trends by Loyalty membership.  <b>4b.</b> Customer distribution by order frequency and loyalty  membership. Green color represents loyalty members and orange highlights non-loyalty members.
></td></tr>
> </table>
>

**Fig. 4a.** shows non-loyalty members are the primary revenue drivers from 2019 through 2020. This has shifted in 2021 highlighting **strong retention and customer value growth** with loyalty program. At the beginning of 2021, loyalty members surspass non-loyalty customers in total revenue. This is supported by a steady increase in average order value (AOV) clearly indicating improved customer engagement. 

In contrast, non-loyalty revenue and AOV has fallen sharply toward the end of 2020 signaling the non-loyalty member's higher volatlity and sensitivity to external factors such as promotions and market conditions.

From mid 2022 onward, loyalty revenue began to decline, eventually falling below non-loyalty revenue by september 2022.  This reversal signals potential engagement fatigue, reduced program attractivenss, and post-pandemic market normalization. While the loyalty program proved effective in driving retention and value in 2021, sustaining engagement over time remains a challenge which will require continuous optimization.

**Fig. 4b.** shows customer distibution by order frequency. There are high proportion (~94%) of one-time buyers.  This siginifies a significant retention gap. Out of the total one-time buyers, 51% are non-loyalty customers and remaining are loyalty. Across all order freuqency segments, non-loyalty customers dominate overall volume. Only 5.2%  of customers make a sceond purchase and a very small proportion reach 3+ orders. This all indicates that loyalty program has not yet effectively translated into strong repeat purchase behavior, highlighting an opportunity to improve lifecycle engagement.

</details>


<details>
  <summary> <b>Key Insights and Recommendations</b> </summary>

 **Key Insights**
 - Rapid acquisiton of non-loyalty customers in 2020 drove short term revenue growth
 - Loylatly program showed clear success in 2021 with improved AOV and retention
 - 2022 decline suggests waning engagment or insufficient program evolution.
 - Extremely high share of one time buyers signals weak customer retention.


**Recommendations**
- Enhance loyalty value proposition by introducing exclusive perks like early access to bestsellers, member only drops, and personalized discounts.
- Re-engage inactive loyalty members with lifecycle campaigns.
- Continuous monitoring of loyalty vs non-loyatly revenue, AOV trends and repeat purchase rates.
- Stabilize  and grow AOV for loyalty members by bundling strategies or optimizing pricing and promotional strategies.


While the available data is not sufficient to make a conclusive decision about loyalty program. The observed trends are clear which shows that loyalty program have strong potential but inconsistent performance. Long term success will depend on continuous iteration, personalization, and deeper integration into the customer journey. 
</details>


### 3. Geographic Performance

<details>
<summary> <b>Click for details and figures</b></summary>

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
>       <b>Fig. 5a. Regional sales performance by revenue, order volume, and average order value (AOV). Inset shows the top country with highest revenue for North America (NA).</b>  <b>5b.</b>  Refund rate by region.
></td></tr>
> </table>
>

**Fig. 5a** shows sales performance by revenue, order volume, and average order value. **North America (NA)** is the dominant regional market and it accounts for apporximately **67% of the total revenue**. **United States (US)** is the primary revenue driver, with **Canada (CA)** as a secondary market. Revenue within NA is heavily skewed towards the US (nine times higher than  CA). Howeve, NA also have relatively higher refund rate compared to other region (Fig. 5b), indicating potential inefficiencies in customer expectations and fulfillment process. This might be the reason impacting the net profitability

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
>       <b>Fig. 6a.</b> Country level sales performance by revenue, order volume, and average order value (AOV). <b>6b.</b>  Pareto Analysis of Revenue contribution by country (with revenue >$10K).
></td> </tr>
> </table>
>

**Fig. 6a** shows that the United states alone contribute **57%** of the  total revenue significantly outperforming all other countries. Notably, the second largest market GB generates **6** times less revenue than the US. Pareto Analysis (Fig. 6b) shows that **top 14 countries contribute **89%** of the total revenue indicating strong geographic concentration. Japan ranks among the top revenue contributors and stands out with the **highest AOV (~$390)** suggesting strong purchasing power, high value customers, and high value market. Revenue is heavily concentrated in a small number of countries with US dominating volume and Japan representing a high value opportunity.

</details>

<details>
  <summary> <b>Key Insights and Recommendations</b> </summary>

**Key Insights**
- **North America (NA)** is the primary revenue driver contributing **67%** of total revenue.
- Revenue distribution is highly concetrated with top 14 countries generating **~89%** of total revenue. **US market (~57%)** outperforms other country by signifcant amount.
- Japan stands out as **high AOV market** indicating high value potential.
- Higher refund rate in NA suggest **potential operational or customer experience challenges**


**Recommendations**
- Continue strategic investment in the US and expand targeted growth initiatives in UK, Canada and Japan.
- Diversify revenue across regions by localize marketing, pricing and scaling in other countries.
- Investigate main drivers of high refunds in North America and optimize product descriptions, sizing, and logistics to reduce return rates.
- Position Japan and other high value markets for premium offerings to maximize AOV

</details>



### 4. Marketing and Operational
<details>
<summary> <b>Click for details and figures (in Progress)</b></summary>

### 4. Marketing Channel Performance

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

- channels vary in revenue contribution, refund rates

optimize marketing ROI

### 5. Operational Performance

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

- Delivery delays impact customer experience. refund likelihood

improve logistics consistency

</details>
