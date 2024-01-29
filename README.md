# SQL-PBI_Customer_Segmentation_and_Sale_Performance

## I. Introduction 

### 1. Business Context

Adventure Works Cycles, a large, multinational manufacturing company, produces and distributes metal and composite bicycles to North American, European, and Asian commercial markets. While its base operation is located in Bothell, Washington, and employs 500 people, several regional sales teams are located throughout the company's market region. In 2000, Adventure Works Cycles bought a small manufacturing plant, Wide World Importers, which is located in Mexico City, Mexico. Wide World Importers manufactures several critical subcomponents for the Adventure Works Cycles product line. These subcomponents are shipped to the Bothell location for final product assembly. In 2001, Wide World Importers became the sole manufacturer and distributor of the touring bicycle product group.
After a successful fiscal year, Adventure Works Cycles is looking to broaden its market share by focusing its sales efforts on the company's best customers, and reducing the cost of sales by reducing production costs.

### 2. Business Question 
 **1.1 Customer segmentation and profiling** 
 
 The sales team needs to be able to extract valuable information from raw data available in the databases to answer questions such as the following:
- What are the early warning signs of problems?
- Who are the best customers across all product lines? With whom should the sales team focus its efforts for building long-term relationships?
- What are customers' issues, categorized according to demographic groups (geographic location, revenue history, and so on)?
- What products are the customers buying and at what rate?

**1.2 Sales performance** 

When analyzing the insights of Sales Performance, the manager will comprehend the trend of the performance of each region through time series analysis, and recognize the region as either the potential one or not. Then, they will be supported to make good decisions for business strategies.

### 2. Dataset

Dataset: adventureworks2019 (public Google BigQuery dataset)

Dataset dictionary: Please reach file "Data Dictionary" attached above

Dataset Schema: https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1

Dataset access:

Log in to your Google Cloud Platform account and create a new project.
Navigate to the BigQuery console and select your newly created project.
In the navigation panel, select "Add Data" and then "Star a project by name".
Enter the project name "adventurework2019"

## II. Apply design thinking mindset
**1. Empathize**
![image](https://i.imgur.com/yE5rLan.png)

**2. Define point of view**
![image](https://i.imgur.com/deLNBkv.png)

**3. Ideate**
![image](https://i.imgur.com/wH0TO4o.png)

**4&5. Prototype and review**
![image](https://i.imgur.com/U3seAdm.png)

## III. Main Process

#### 1. Extract data with Google Bigquery

**Output total revenue of each subcategory and category product by quarter/year**
![image](https://i.imgur.com/2t115d8.png)


## IV. Insights
#### 1. Customer Segmentation - Customer Count
- The Champions group(8.8% of customers) has the highest revenue, at 73.8 million, accounting for 67% of the total revenue. For each subcategory, Champion customers are consistently the highest spenders. However, customer champions only account for 9.55% of the total profit.
- Accessories is a promising category, with explosive revenue growth of 45% in Q2 2013. The industry boasts a profit margin of 50% and is not incurring any losses. Champions and Potential Loyalist groups. The Champion and Potential Loyalist customer groups make the highest purchases within this sector, contributing to 56% of the revenue and 47% of the total profit. Champion customers buy helmets and bike racks for most, 75% revenue and 73% sum of profits. Tire and tubes, helmets account for 73% total of revenue and 74% of total profit in Potential Loyalist 
- Champion and Cannot Lose Them customers account for a significant portion of the revenue in the three industry groups: Bikes, Components, and Clothing, particularly dominating with 99% of the revenue in the Components sector, totaling 11.6 million dollars.
- Promising and new customers account for 15.08% and 14.86%, respectively, making them the two customer groups with the highest share.

#### 2. Geographical distribution of customers
- Promising and new customers account for 15.08% and 14.86%, respectively, making them the two customer groups with the highest share
- For Promising customers in the Americas, there are 1600 customers generating $1.72 million in revenue, constituting 62% of the total revenue from Promising customers.
- Promising and New customers form the most dynamic and freshest customer segment, comprising the largest share in customer classification (30%). The Western United States and Europe are regions with high proportions of new and promising customers, with rates of 37% for Southwest US, 38% for Northwest, 36% for France, 28% for the UK, and 37% for Germany
- Regions with fewer customers, such as the Northeast, Southeast US, and South America, will have a high percentage of Champion customers (approximately 45% to 55% of customers).
- In both the Canadian and Australian markets, there are two major customer segments: Prospective Customers and Loyal Customers. In the Canadian market, Prospective Customers constitute a higher percentage, accounting for 44.5% of the total customer base (including PL, P, and New). Conversely, in the Australian market, the percentage of Loyal Customers is higher, making up 49% of the total customer base (including L, AR, and Champions).

#### 3. 
- The company's bicycle production figures consistently demonstrate promise each quarter, with most quarters showing positive growth. However, there is a decline in the fourth quarter. Regarding the company's profits, the quarter experiences negative growth, while the remaining quarters all exhibit positive growth.
- The company's bicycle production figures consistently indicate promise across each quarter, with most quarters experiencing positive growth. However, there is a decline in the fourth quarter. Concerning the company's profits, the fourth quarter shows negative growth, while the remaining quarters all exhibit positive growth. Particularly, the third quarter demonstrates robust growth in both revenue and profit, with a 423.57% increase and $241.445 million in 2011 and a 16.22% increase and $484.05 million in 2013.
- The regions with consecutive revenue and profit growth over the years are Australia, France, Germany, and the UK.
- The Australian market is a market with six consecutive quarters of revenue growth. Among these, quarters 1 and 4 show lower growth compared to quarters 2 and 3. Quarters 1 and 4 experience growth in the range of 11-23%, while quarters 2 and 3 exhibit growth in the range of 36-56%.
- In the Australian market, bicycles contribute over 90% to both revenue and profit across quarters. During quarters 3-4 of 2013, mountain bikes experienced a decline in revenue (-0.86% and -4.89%) but recovered in quarter 1 of 2014 with a growth of 23.11%. However, road bikes, despite having a decreasing revenue growth trend (47% and 23% in quarters 3-4 of 2013 and 1.74% in quarter 1 of 2014), still contribute significantly to the overall revenue.
- Touring bikes were introduced in Q2 2013, showing continuous positive revenue growth from Q2 2013 to Q1 2014. In Q1 2014, revenue from touring bikes accounted for 41.25% of the total bike revenue.
- The Accessories sector in Australia is also a promising industry. Introduced for the first time in Q2 2013, it experienced an explosive revenue surge in Q3 2013 with a remarkable increase of 322%. In the subsequent quarters, the revenue continued to grow, albeit at a milder pace. Among the various products in this sector, Tire and Tubes and Helmets hold the largest market share, comprising approximately 60% of the total revenue since Q2 2013. Both product categories have shown consecutive positive revenue growth from Q3 2013 onwards.
- For the Accessories sector in France, there is a significant decline in revenue every fourth quarter. However, the fenders product subcategory exhibits consecutive positive revenue growth from Q2 2013 to Q1 2014.
- In France, the mountain bikes category shows continuous revenue growth across quarters. Road bikes used to account for the majority of bicycle revenue (>63%) in previous quarters. However, since the introduction of touring bikes, their market share has decreased to 30%. Subsequently, touring bikes have become the largest market share holder, representing approximately 40% of the total revenue.
- For bicycles in Germany, road bikes experience a decline in revenue each quarter, making way for mountain and touring bikes. Mountain bikes exhibit impressive revenue and profit growth, consistently growing positively for six consecutive quarters. In contrast, touring bikes show a slight decrease in revenue in Q4 2013 (-10.84%), with a substantial decline in profit (-736.28%).
- The UK market experiences a decline in sales at the beginning and end of the year, while strong growth is observed in quarters 2 and 3. Particularly, touring bikes emerge as a highly promising product category with consistently increasing revenue. However, the profit for this product category sees a significant decrease.
- 
