# Global-Superstore-Sales-Analysis-Dashboard
This project showcases my ability to use Power BI to transform raw sales data into meaningful business insights. Using the Global Superstore dataset, I analyzed global sales, profit, and customer trends across regions, product categories, and customer segments to identify key performance patterns and opportunities for business growth.

### **Raw Data Link:**  
[Download Global Superstore Dataset (CSV)](https://github.com/shazlanamirul8/Global-Superstore-Sales-Analysis-Dashboard/raw/main/Sample-superstore.csv)

### Transform Data
There was minimal transformation required for the raw dataset.  
I performed basic cleaning and added a few calculated columns in **Power Query** for better analysis and visualization.

**New Columns Added:**
- **Year (Order Date):** To analyze yearly sales and profit trends  
  ```DAX
  Year = Date.Year([Order Date])
- **Month (Order Date):** To observe seasonal and monthly performance
  ```DAX
  Month = Date.monthname([Order Date])
- **Sales After Discount:** To evaluate the effect of discounts on total revenue
  ```DAX
  Sales After Discount = [Sales] * (1-[discount])
- **Profit Margin:** To measure profitability across categories and regions  
  ```DAX
  Profit Margin = [Profit] / [Sales]
    
These transformations ensure the dataset is structured for accurate time-series and profitability analysis.
