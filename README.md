# Project Name: Superstore Data Exploration Report - In-Depth Analysis
This report offers a detailed analysis of the Superstore dataset. It delves into data exploration, cleaning, transformation, and visualization techniques used in Power BI.

## Data Description
The Superstore dataset offers a wealth of information on product sales, encompassing 9994 rows and 21 columns containing attributes like:

- **Row ID**: A unique identifier for each row
- **Order ID**: The unique identifier for the order
- **Order Date**: The date when the order was placed
- **Ship Date**: The date when the order was shipped
- **Ship Mode**: The shipping mode selected for the order
- **Customer ID**: The unique identifier for the customer
- **Customer Name**: The name of the customer
- **Segment**: The customer segment (e.g., Consumer, Corporate)
- **Country**: The country where the customer is located
- **City**: The city where the customer is located
- **State**: The state where the customer is located
- **Postal Code**: The postal code of the customer's location
- **Region**: The region where the customer is located
- **Product ID**: The unique identifier for the product
- **Category**: The category of the product
- **Sub-Category**: The sub-category of the product
- **Product Name**: The name of the product
- **Sales**: The sales amount of the product
- **Quantity**: The quantity of the product ordered
- **Discount**: The discount applied to the product
- **Profit**: The profit made from the product




## Data Cleaning and Transformation in Power BI
- **Data Cleansing**: A thorough examination revealed no duplicate values within the dataset.
- **Data Type Conversion**: The postal code data type was transformed from numerical to text format.
- **Column Removal**: Two columns were eliminated:
  - **Row ID**: As it serves as a unique identifier for each row but doesn't contribute directly to sales insights.
  - **Country**: Since all entries belonged to the United States, this column was removed to streamline the focus.
- **Order Date Transformation**: To extract valuable insights from the order date, a multi-step process was implemented:
  - **Day of Week (Numerical)**: A new column was created to represent the numerical day of the week (ranging from 0 for Sunday to 6 for Saturday).
  - **Day Name Extraction**: The full day name (e.g., Monday) was extracted from the order date for potential future analysis.
  - **Day Name Abbreviation**: To condense information, the first three letters of the day name (e.g., Mon for Monday) were extracted as a separate column.

## Data Visualization - Unveiling Trends and Patterns
The visualizations were  crafted in Power BI and categorized into two distinct reports: Periodic Report and Location Report.

**Periodic Report**
- **Line Chart - Sales Trend Over Months**: This dynamic line chart showcases the sales trajectory across various months within the dataset, enabling identification of seasonal trends or cyclical patterns.
- **Ribbon Chart - Customer Segment Ranking**: The ribbon chart provides a visually compelling illustration of how customer segments (Consumer, Corporate, etc.) rank against each other throughout the months. This facilitates understanding of which customer segment contributes most significantly to sales during specific periods.
- **Column Chart (1) - Average Sales by Day of Week**: This column chart delves deeper, revealing the average sales amount for each day of the week. This visualization sheds light on potential variations in buying behavior across weekdays and weekends.
- **Column Chart (2) - Number of Transactions by Day of Week**: This column chart complements the previous one by portraying the number of transactions that occur on each day of the week. By analyzing both average sales and transaction volume, we can gain a more comprehensive understanding of customer buying patterns throughout the week.

**Location Report**
- **Column Chart (1) - Top and Bottom Performing States**: This column chart prioritizes the top 5 and bottom 5 states based on their total sales figures. This visualization allows for quick identification of high-performing and low-performing regions in terms of sales.
- **Refined Column Chart (Consideration)**: It's essential to assess the visualization tool's capabilities. Depending on the software, this second column chart might be redundant if it simply mirrors the top and bottom state breakdown from the previous chart.
- **Table - Top 10 States and Transaction Shipment Percentage**: This table prioritizes the top ten states and displays the percentage of transaction shipments for each. This visualization provides valuable insights into the geographical distribution of sales and potential areas for targeted marketing efforts.





