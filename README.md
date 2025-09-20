# Sales Dashboard and Forecasting — Power BI

_Analyzing sales performance, regional trends, and forecasted growth to empower data-driven business decisions using Power BI._

---

## Table of Contents
- <a href="#overview">Overview</a>
- <a href="#objectives">Objectives</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#data-cleaning--transformation">Data Cleaning & Transformation</a>
- <a href="#dax-queries">DAX Queries</a>
- <a href="#insights">Insights</a>
- <a href="#forecast">Forecast</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#file-structure">File Structure</a>
- <a href="#notes">Notes</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project delivers an interactive sales dashboard and a 30-day sales forecasting model built using **Microsoft Power BI** on the `SuperStore Sales Dataset` sourced from Kaggle. The dashboard empowers decision-makers to explore sales performance, regional trends, product categories, and timelines, with visual forecasting to aid business planning.

---

<h2><a class="anchor" id="objectives"></a>Objectives</h2>

- Provide comprehensive sales and profit visualizations.
- Enable users to explore sales by region, product category, shipping, and payment mode.
- Implement a short-term sales forecast leveraging Power BI’s built-in time series features.
- Contribute to business success by applying data analysis techniques, with a special focus on time series analysis, to generate valuable insights and accurate sales forecasting.

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Microsoft Power BI for data transformation, visualization, DAX calculations, and forecasting.
- DAX language for custom calculations and new column creation.

---

<h2><a class="anchor" id="data-cleaning--transformation"></a>Data Cleaning & Transformation</h2>

Data was cleaned and transformed within Power BI’s Query Editor :

1. Deleting *Empty Columns* present in data named as **ind1** and **ind2**

   ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/1%20(%20delete%20empty%20columns%20).jpg)

3. Replacing Values in **Returns** Column ( changing *#N/A* to *0* to maintain consistency as other option is *1* )

   | Step 1 | Step 2 | Step 3 |
   |---------|---------|---------|
   | ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/2%20(%20replace%20na%20).jpg) | ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/2.1.jpg) | ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/2.2.jpg) |

3. Applied Steps

   ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/4%20(%20new%20column%20using%20DAX%20).png)

---

<h2><a class="anchor" id="dax-queries"></a>DAX Queries</h2>

Key DAX calculations include :

1. Creating **new column** named **Avg-Delivery** to store the number of days between *Order Date* and *Ship Date*

   ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/4%20(%20new%20column%20using%20DAX%20).png)
   

2. Creating a **new secondary table** named *Sales_Forecast* using **Order Date** and **Sales** columns of original data to support forecasting analysis..

   ![Image Alt](https://github.com/Adhyan-1404/dashboard-superstore-dataset-powerbi/blob/715ce8f085a1456cab10596468390a6e035dc835/Image%20Assets/5%20(%20Table%20).jpg)

---

<h2><a class="anchor" id="insights"></a>Insights</h2>

Based on data from 2019 and 2020 :

#### 1. Overall Performance across both years :
   - Total Sales - **1.57M**
   - Total Profit - **175.3K**
   - Average Time Taken to Ship Items - **4 days**
   - Total Quantity of Items Sold - **22k**

#### 2. Sales by Region :
   - Top Performing Region - **West**
   - Least Performing Region - **South**

#### 3. Sales by Segment :
   - Top Performing Segment - **Consumers**
   - Least Performing Segment - **Home Office**

#### 4. Category-wise and Sub-Category-wise Sales :
   - Top Performing Category - **Office Supplies**
   - Top Performing Sub Category - **Phones**
     
#### 5. Year-over-Year Trends :
   - Monthly Sales by YoY (2019 vs 2020) :
     
     - **2020 outperformed 2019** consistently across the year.
     - Peaked in **September**, **November** and **December.**
       
   - Monthly Profit by YoY (2019 vs 2020) :
     
     - **2020 outperformed 2019** across the year except in **April** and **February**.
     - Peaked in **March**, **October** and **December.**

#### 6. Preferred Shipping Mode :
   - Top Preferred Shipping Mode - **Standard Class**

#### 7. Preferred Payment Mode :
   - Top Preferred Payment Mode - **Cash on Delivery**

#### 8. Sales and Profir by State :
   - **California**, **Texas**, and **New York** are highest contributers.

### Summary Insights :-

- Significant sales growth is localized to West and Consumer segment.
- Inventory management should prioritize Phones, Chairs, and Binders.
- End-of-year is critical for sales spikes and campaign planning.
- Shipping and payment preferences remain stable with Standard Class and Cash on Delivery dominant.

---

<h2><a class="anchor" id="forecast"></a>Forecast</h2>

Over the next 30 days, projected sales are expected to average approximately 3,500 units per day. This forecast was developed using historical sales data and seasonality patterns observed over the past two years.

- A temporary decline is anticipated at the beginning of the forecast period, followed by a phase of growth. Sales are then expected to stabilize toward the end of this period.

- Similar trends have been observed in previous periods, where short-term declines were often followed by recovery and strong performance, particularly during mid-year and end-of-year months. For example, significant sales spikes occurred in June and December during both 2019 and 2020.

**Note :** This forecast is based solely on historical trends and may not fully account for external market changes or unforeseen events. Actual sales may vary.

---

<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

