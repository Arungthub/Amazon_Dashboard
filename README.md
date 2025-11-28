#  Amazon Sales Analytics – Power BI Dashboard

This repository contains an interactive **Amazon Sales Analytics Dashboard (AM_PowerBI.pbix)** built in Microsoft Power BI.
The dashboard provides insights into sales performance, product trends, customer behavior, territory insights, and return analysis using a clean star-schema data model.

---

##  Dashboard Preview

### ** Sales Report **

Here is a preview of the main dashboard page:

![Monthly Sales Report](https://github.com/Arungthub/Amazon_Dashboard/blob/main/Screenshot%202025-11-28%20095703.png?raw=true)

---

##  Dashboard Features

The Monthly Sales Report page contains:

* **Total Orders by Category Name** — Treemap visualization for categories like Accessories, Bikes, Clothing.
* **Total Orders by Sub-Category Name** — Bar-chart view of sub-category order counts (e.g. Tires & Tubes, Helmets, Road Bikes, Mountain Bikes, etc.).
* **Product Distribution by Profit / Loss** — Dynamic table listing each product with a “profit or loss” calculation, powered by a toggle.
* **Profit  Opportunity Loss Toggle** — A switch that allows users to toggle view between Profit and Opportunity Loss across visuals and KPIs.
* **Key KPI Cards** — Displaying Total Profit (vs goal), Total Returns, Opportunity Loss, and related metrics.
* **Top 3 Performer / Loser Products** — Highlights top performing or loss-making products dynamically.
* **Global Map Visualization** — Displays geographic distribution of sales/returns across continents (North America, Europe, Asia, etc.), giving territory-level insights.

---

##  Data Model Overview

The data model uses a **star schema** for optimized performance and clean relationships.

### Fact Tables

* **AM_Sales** — Main sales transactions
* **Amazon_Returns** — Return/return-related transactions

### Dimension Tables

* **Amazon_Products**
* **Amazon_Product_Subcategories**
* **Amazon_Product_Categories**
* **Amazon_Customers**
* **Amazon_Territories**
* **Amazon_Calendar** (Date table)
* **Profit_Loss Toggle** (helper table for toggling between Profit and Opportunity Loss view)

---

##  Column Reference (Data Dictionary)

### **AM_Sales**

* CustomerKey
* OrderStatus
* OrderNumber
* OrderQuantity
* ProductKey
* ProductPrice
* PurchaseCost
* SalesAmount
* ReturnStatus

### **Amazon_Products**

* ModelName
* ProductColor
* ProductDescription
* ProductName
* ProductPrice
* ProductSize
* ProductSKU
* SubCategoryKey

### **Amazon_Product_Subcategories**

* ProductSubcategoryKey
* ProductSubcategoryName
* SubcategoryImage

### **Amazon_Product_Categories**

* CategoryName
* ProductCategoryKey

### **Amazon_Customers**

* Age
* AnnualIncome
* BirthYear
* Education
* Gender
* CustomerKey
* EducationLevel
* FirstName
* LastName
* FullName

### **Amazon_Territories**

* Continent
* Country
* Region
* SalesTerritoryKey

### **Amazon_Returns**

* ProductKey
* ReturnDate
* ReturnStatus
* ReturnReason
* ReturnQuantity
* TerritoryKey
* OpportunityLoss
* OpportunityLossTargets

### **Amazon_Calendar**

* Date

### **Profit_Loss Toggle** (helper table)

* Values

---

##  Tools & Technologies Used

* **Microsoft Power BI Desktop**
* **Power Query** (for data shaping and transformations)
* **DAX** (for calculated measures, KPIs, toggles)
* **Star Schema Data Modeling**


---

##  How to Use This Project

1. Download the Pbix file .
2. Open **AM_PowerBI.pbix** with Power BI Desktop.
3. Use slicers and filters to explore the dashboard.
4. Toggle between Profit and Opportunity Loss to analyze different views.


---

##  Future Enhancements

* Add forecast & predictive analytics modules (sales forecasting, demand prediction).
* Integrate Row-Level Security (RLS) for user-based data access.
* Add drill-through pages (customer details, product returns, territory performance).
* Live integration with cloud data sources (Azure / Dataverse / SQL) for real-time analytics.

---

## Contact

**Arun Kumar T**
📧 Email: [arunkumartekumani46@gmail.com](mailto:arunkumartekumani46@gmail.com)
🌐 Portfolio: [https://arungthub.github.io/My-Portfolio/](https://arungthub.github.io/My-Portfolio/)
📍 Location: Bangalore, India

---

