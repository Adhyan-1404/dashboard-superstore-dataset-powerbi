# Data Cleaning and Transformation before working on Dashboard

1. Deleting *Empty Columns* present in data named as **ind1** and **ind2**

   ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/1%20(%20delete%20empty%20columns%20).jpg)

3. Replacing Values in **Returns** Column ( changing *#N/A* to *0* to maintain consistency as other option is *1* )

   | Step 1 | Step 2 | Step 3 |
   |---------|---------|---------|
   | ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/2%20(%20replace%20na%20).jpg) | ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/2.1.jpg) | ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/2.2.jpg) |

3. Applied Steps

   ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/3.jpg)


# Dax Queries

1. Creating **new column** named **Avg-Delivery** to store the number if days between *Order Date* and *Ship Date*

   ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/18461eb99664e3fabc14014bcdea59e2525fc20c/Dashboard%201/Image%20Assets/4%20(%20new%20column%20using%20DAX%20).png)

2. Creating a **new secondary table** named *Sales_Forecast* using **Order Date** and **Sales** columns of original table to forecast sales based on data.

   ![Image Alt](https://github.com/Adhyan-1404/Power-BI-Projects/blob/8cf0ba85a1951a0c597054270c39ab1ab2e83733/Dashboard%201/Image%20Assets/5%20(%20Table%20).jpg)

