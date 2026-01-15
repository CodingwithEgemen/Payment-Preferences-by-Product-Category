# 📊 Sales Performance & Payment Method Analysis  
<img width="600" height="400" alt="kapak" src="https://github.com/user-attachments/assets/309c6f99-5325-4a32-95fa-c1f228fb325a" />


## 🔍 Project Overview
This project analyzes customer payment method preferences across product categories and examines differences between weekday and weekend sales behavior using Google Sheets. The objective is to demonstrate how spreadsheet-based tools can be used to perform data integration, transformation, and analytical reporting tasks that are conceptually equivalent to SQL joins and BI dashboards, without relying on external analytics platforms.

## 📁 Data Sources
The analysis is based on three CSV datasets:

👥 **Customers**  
Includes customer identifiers and city information.

🛒 **Products**  
Includes product identifiers, product names, categories, brands, and unit prices.

🧾 **Sales**  
Includes transactional data such as sale ID, customer ID, product ID, quantity, day of week, sales channel, and payment method.

Each dataset was uploaded into Google Sheets as a separate worksheet.

## 🔧 Data Preparation & Integration
CSV files were imported into Google Sheets and consolidated into a single analytical table using **IMPORTRANGE**. The Sales dataset was used as the base table. **XLOOKUP** was applied to enrich the sales data by retrieving city information from the Customers dataset and category, brand, and price information from the Products dataset. This approach follows a **LEFT JOIN** logic similar to relational databases and ensures that all sales records are preserved while related attributes are added.

## 🧮 Calculated Fields
To support analysis, additional calculated fields were created:

💰 **Revenue**  
Calculated as *Quantity × Price* to represent the financial value of each transaction.

📅 **DayType**  
Derived from the *day_of_week* field to classify each sale as either **Weekday** or **Weekend**, enabling time-based comparisons.

## 📈 Analysis & Deliverables
A pivot table was created with **Product Category** as rows, **Payment Method** as columns, **Quantity aggregated as SUM**, and **DayType** used as a filter. This structure enables direct comparison of payment method preferences across categories and between weekdays and weekends.

📊 Bar and column charts were created based on the pivot table. Visualizations dynamically update according to the selected DayType filter.

## 🔑 Key Insights
💳 Payment method preferences vary across product categories.  
📈 Card payments show increased usage during weekends.  
💵 Cash payments are more common on weekdays for certain categories.  

These patterns indicate that **payment-based and day-specific sales strategies** can be optimized to improve campaign effectiveness.

## 🛠️ Tools & Skills Demonstrated
- Google Sheets  
- IMPORTRANGE  
- XLOOKUP  
- Calculated fields  
- Pivot tables and charts  
- Data modeling and analysis  
- SQL-like analytical thinking  


## ✅ Conclusion
- This project demonstrates the ability to transform raw transactional data into meaningful business insights using spreadsheet-based tools. It highlights practical skills in data integration, analytical reasoning, and data visualization that are directly applicable to real-world business scenarios.

## 👤 Author
Egemen Efe SAHIN
