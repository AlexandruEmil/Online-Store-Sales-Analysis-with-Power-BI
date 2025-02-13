# Online-Store-Sales-Analysis-with-Power-BI
This just an example of the store 


This project is focused on the analysis of sales data from an online store, using Power BI to create interactive dashboards and valuable business insights. The project covers key metrics and visualizations, offering a clear view of product performance, customer behavior, and regional sales trends.

📁 Project Structure

   Data Sources:

    Sales Table: Contains transactional data (Sales_ID, Product_ID, Customer_ID, Date, Total_Amount).
    Products Table: Includes product information (Product_ID, Product_Name, Category, Price_per_Unit).
    Customers Table: Stores customer details (Customer_ID, Customer_Name, Region, Client_Type).

🧮 Key Metrics (DAX Measures)

  The following DAX measures were created to analyze sales data:

   Total Revenue:

    Total_Venit = SUM(Sales[Total_Amount])
    Calculates the total revenue from all sales transactions.

   Unique Customers Count:

    Nr_Clienți = DISTINCTCOUNT(Sales[Customer_ID])
    Counts the number of unique customers.

   Average Order Value:

    Valoare_Medie_Comanda = AVERAGE(Sales[Total_Amount])
    Calculates the average revenue per order.

📊 Visualizations and Dashboards

   Top Selling Products:

    Visualization: Bar Chart.

   Configuration:

    Axis: Product_Name
    Values: Total_Venit
    Insights: Shows the best-performing products based on total sales.

   Monthly Trends:

    Visualization: Line Chart.

   Configuration:

    Axis: Date (grouped by month/year).

    Values: Total_Venit.

    Insights: Highlights sales trends over time to identify seasonality.

  Sales by Region:

    Visualization: Map Chart.

  Configuration:

    Location: Region
    Size: Total_Venit
    Insights: Displays sales performance across different regions.

🔘 Interactive Filters (Slicers)

    Date Slicer: Allows filtering data by date or time periods.

    Category Slicer: Filters sales data by product category.

    Client Type Slicer: Enables filtering based on customer type (e.g., new or returning customers).

🛠️ How to Run the Project

    Load Data: Ensure the data tables (Sales, Products, Customers) are imported into Power BI. 

  Create Data Relationships:

    Sales[Product_ID] linked to Products[Product_ID].
    Sales[Customer_ID] linked to Customers[Customer_ID].

    Add DAX Measures: Copy the provided DAX formulas into Power BI.
    Build Visualizations: Follow the visualization configurations above to create the necessary charts.
    Add Slicers: Insert slicers to filter data interactively.

📈 Business Insights

    Top-selling products reveal which items drive the most revenue.\
    Seasonal trends help identify peak sales periods for better inventory planning.\
    Regional analysis uncovers high-performing regions and potential markets for growth.

