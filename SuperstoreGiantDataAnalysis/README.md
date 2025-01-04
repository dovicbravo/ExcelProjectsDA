# Superstore Giant Data Analysis

*By Dovic Bravo*

## Introduction 

In this data analysis project, Superstore Giant business would like to understand which products, regions, categories, and customer segments they should target or avoid.

### Questions to Analyze:

To understand the following:

1. **Which categories and products generate the highest profit?**
2. **The effect of discount on sales and profit**
3. **Which region and segment are the most profitable?**
4. **Applying a Pareto Analysis to identify which products the business should pay more attention to**

### Skills Used

The following Excel skills were utilized for analysis:

- **📊Pivot Tables**
- **📈 Pivot Charts**
- **🧮 DAX (Data Analysis Expressions)**
- **🔍 Power Query**

## Dataset

### Data Information

The dataset used in this project was from kaggle [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final).

The data consists of the following Variables/Columns:

![datavariables.png](/SuperstoreGiantDataAnalysis/images/datavariables.png)

## Data Cleaning

### Loading the Data

- I used **Power Query** to extract the original data (`Sample - Superstore.csv`).

![ETL.png](/SuperstoreGiantDataAnalysis/images/ETL.png)

- The variables are already in correct data type and columns are clean. I duplicated the original data and removed the columns: Row ID, Customer ID, Customer Name, Postal Code, and Product ID from the duplicated data because they will not be used in this analysis.

![ETL2.png](/SuperstoreGiantDataAnalysis/images/ETL2.png)

## Data Analysis

I used **Pivot Table** to summarize, analyze, and visualize the dataset.

In this data analysis, **Comparison, Ranking, and Pareto Analysis** were used.

**Comparison Analysis**
  - Comparing the value of one item against another
  - Understanding which value is the highest and the lowest and how much larger one value to another
  - Used column and bar graphs

**Ranking Analysis**
  - Understanding the ranking order of items
  - Perform Top/Bottom 10 analysis
  - Calculating rankings

**Pareto Analysis**
  - Recognizing disproportional relationships exist between items
  - 80/20 rule
  
### 📊 Products and Categories

I created Key Metrics to measure the performance of the business. I also created a DAX to calculate the overall Profit Ratio of the business.

![keymetrics.png](/SuperstoreGiantDataAnalysis/images/keymetrics.png)

I created a chart of Total Sales and Profit

![pac_totalsalesandprofit.png](/SuperstoreGiantDataAnalysis/images/pac_totalsalesandprofit.png)

I created a chart of Average Profit per Sub Category.

![pac_avergaeprofit.png](/SuperstoreGiantDataAnalysis/images/pac_averageprofit.png)

### 💡 Insights:

Based on the charts, the Technology category demonstrates the highest levels of both sales and profit, indicating it as a key driver of revenue for the Superstore Giant business. Within this category, Copiers generate the highest profit, suggesting a need for strategic focus and resource allocation to further capitalize on this segment.

Conversely, the Furniture category is underperforming in terms of profitability, with particular losses observed in the Tables and Bookcases Sub-Category, both of which report negative profit margins. This highlights a need for review and potential restructuring in this category to address inefficiencies and improve financial performance.

### 📊 Sales and Proft by Discount

I created a chart where the Average Discount per Category is combined with the Total Profit per Category.

![spd_averagediscount.png](/SuperstoreGiantDataAnalysis/images/spd_averagediscount.png)

### 💡 Insights:

Based on the chart, the Technology category achieved the highest sales while maintaining the lowest average discount rate, suggesting a strong demand for products in this category with minimal reliance on promotional pricing. In contrast, the Furniture category recorded the highest average discount rate; despite the significant discount, the total sales for furniture fall in the middle range, indicating that deeper discounts may be a strategy to stimulate demand in this category.

A negative correlation is observed between the total sales and the average discount percentage. Categories with higher discounts (e.g., Furniture) tend to have lower sales compared to categories with lower discounts (e.g., Technology). Furniture Category may rely heavily on discounts to drive sales, which could impact profitability margins if discounts are too deep.

### 📊 Region

I created a chart showing the Total Sales and Profit per Region.

![r_totalesalesandprofit.png](/SuperstoreGiantDataAnalysis/images/r_totalesalesandprofit.png)

I created a chart where Average Discount per Region combined with Total Sales per Region.

![r_averagediscount.png](/SuperstoreGiantDataAnalysis/images/r_averagediscount.png)

I created a chart showing Total Profit per Region by Category.

![r_profitbyregion.png](/SuperstoreGiantDataAnalysis/images/r_profitbyregion.png)

I created a chart showing the Top 10 State with the highest profit.

![r_state.png](/SuperstoreGiantDataAnalysis/images/r_state.png)

### 💡 Insights:

Based on the charts,the Western and Eastern regions are generating the highest profit while maintaining low average discount rates, indicating effective pricing strategies in these areas. In contrast, the Central region applies the highest average discounts but fails to generate profit, particularly within the Furniture category, which reports negative profitability.

Additionally, the states of California and New York, located within the Western and Eastern regions respectively, contribute the highest profit by state. This further underscores the strong performance of these regions and suggests that they may serve as benchmarks for optimizing strategies in underperforming regions.

### 📊 Segment

I created a chart of Total Sales and Profit by Segment

![s_totalsalesandprofit.png](/SuperstoreGiantDataAnalysis/images/s_totalsalesandprofit.png)

I created a chart of Total Profit by Segment per Region

![s_totalprofitbysegment.png](/SuperstoreGiantDataAnalysis/images/s_totalprofitbysegment.png)

I created a shart showing Average Discount combined with Total Sales per Region

![s_totalsalesbydiscount.png](/SuperstoreGiantDataAnalysis/images/s_totalsalesbydiscount.png)

### 💡 Insights:

Based on the charts, the Consumer segment is the most profitable, achieving the highest profit margin with an average discount of 15.5%. In contrast, the Home Office segment reports the lowest profit despite maintaining a slightly lower average discount of 14.5%. This suggests that factors beyond discounting, such as product mix or sales volume, may be impacting the profitability of the Home Office segment and require further investigation.

### 📊 Pareto Analysis

