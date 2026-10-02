# 🛒 Blinkit Sales & Operations Analytics Dashboard | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Analytics-F2C811?style=for-the-badge\&logo=powerbi\&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data-Analytics-blue?style=for-the-badge)
![SQL](https://img.shields.io/badge/SQL-Data%20Preparation-orange?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Project-black?style=for-the-badge\&logo=github)

---

## 📌 Project Overview

This project is an end-to-end **Blinkit Sales & Operations Analytics Dashboard** developed using **Microsoft Power BI**.

The objective of this project is to transform business data related to **orders, customers, products, delivery, inventory, marketing, ratings, and customer feedback** into an interactive Business Intelligence solution.

The dashboard provides a centralized view of business performance and enables users to analyze key areas such as:

* Sales performance
* Order trends
* Product performance
* Customer behavior
* Delivery operations
* Inventory
* Marketing performance
* Customer ratings and feedback

The project demonstrates how raw business data can be transformed into meaningful visual insights to support **data-driven business decisions**.

---

## 🎯 Business Objective

The primary objective of this project is to build a centralized Business Intelligence solution that can help answer important business questions such as:

* How are sales and order volumes performing?
* Which products and categories contribute most to sales?
* What are the major customer purchasing patterns?
* How does delivery performance vary across different periods or locations?
* Which products require inventory attention?
* What are the major customer rating and feedback trends?
* How can marketing performance be analyzed alongside sales?
* Which areas may require operational improvement?

The dashboard converts raw business data into an interactive reporting environment where users can explore trends, compare performance, and identify business opportunities.

---

## 🛠️ Tools & Technologies

| Tool / Technology      | Purpose                                                     |
| ---------------------- | ----------------------------------------------------------- |
| **Microsoft Power BI** | Dashboard development, visualization and business reporting |
| **Power Query**        | Data cleaning and transformation                            |
| **DAX**                | Measures and analytical calculations                        |
| **Data Modeling**      | Building relationships between business entities            |
| **SQL**                | Data querying and analytical preparation                    |
| **Excel / CSV**        | Source data handling                                        |
| **GitHub**             | Project documentation and portfolio presentation            |

---

## 🗂️ Data Model

The Power BI project uses a relational data model consisting of multiple business entities.

### Main Tables

#### 📦 Orders

Contains order-level transaction information used for:

* Order analysis
* Order trends
* Customer-order relationships
* Order status analysis
* Time-based analysis

#### 🛍️ Order_item

Contains individual items associated with orders and supports:

* Product-level sales analysis
* Quantity analysis
* Item-level performance
* Product contribution

#### 🏷️ Products

Contains product-related information used for:

* Product performance analysis
* Category analysis
* Product-level sales analysis
* Product comparison

#### 👥 Customer

Contains customer-related information used for:

* Customer analysis
* Customer behavior analysis
* Customer segmentation
* Customer contribution analysis

#### 💬 Customer_feedbacks

Contains customer feedback information used for:

* Customer satisfaction analysis
* Feedback analysis
* Rating analysis
* Identifying customer experience trends

#### 🚚 Delivery

Contains delivery-related information used for:

* Delivery performance analysis
* Fulfillment analysis
* Operational performance
* Delivery trends

#### 📦 Inventory

Contains inventory-related information used for:

* Stock analysis
* Product availability
* Inventory monitoring
* Inventory planning

#### 📢 Marketing

Contains marketing-related information used for:

* Marketing performance analysis
* Campaign analysis
* Marketing and sales comparison
* Business performance analysis

#### 🗃️ Master_Table

Contains master/reference information used within the analytical model to support reporting and analysis.

#### 📁 Folder

Supporting organizational/reference information used within the Power BI model.

#### 🏷️ Category_Icon

Supporting category-related information used for dashboard presentation and categorization.

#### ⭐ Ratings_Icon

Supporting rating-related information used for dashboard presentation and rating analysis.

---

## 🔄 Data Preparation Process

The data preparation process follows a structured Business Intelligence workflow:

```text
Raw Business Data
       ↓
Data Import
       ↓
Data Cleaning
       ↓
Data Transformation
       ↓
Data Validation
       ↓
Data Modeling
       ↓
DAX Measures
       ↓
Interactive Dashboard
       ↓
Business Insights
```

### Data Cleaning & Transformation

Power Query was used to prepare the data for analysis.

The preparation process includes activities such as:

* Removing unnecessary columns
* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing values
* Transforming raw data
* Preparing tables for analysis
* Validating data consistency
* Creating a structured analytical dataset

---

## 🧩 Data Modeling

A relational data model was created in Power BI to connect different business entities.

The model brings together transactional, customer, product, delivery, inventory, marketing, and feedback information to support cross-functional analysis.

The high-level analytical structure can be represented as:

```text
                  Customer
                     │
                     ↓
Orders ─────────→ Order_item ─────────→ Products
  │                                      │
  │                                      ├────→ Inventory
  │                                      │
  │                                      └────→ Category
  │
  ├────────→ Delivery
  │
  └────────→ Customer_feedbacks

Marketing
    │
    ↓
Business / Sales Performance
```

The purpose of the model is to create a structured reporting layer where different business dimensions can be analyzed together.

---

## 🧮 DAX Measures

DAX (Data Analysis Expressions) was used in Power BI to create analytical measures and support dynamic reporting.

The dashboard can use measures for metrics such as:

* Total Sales
* Total Orders
* Total Customers
* Total Products
* Average Order Value
* Average Rating
* Quantity Sold
* Sales by Category
* Sales by Product
* Order Trends
* Customer Performance
* Delivery Performance

### Example DAX Measures

```DAX
Total Sales =
SUM(Order_item[Sales])
```

```DAX
Total Orders =
DISTINCTCOUNT(Orders[Order_ID])
```

```DAX
Total Customers =
DISTINCTCOUNT(Customer[Customer_ID])
```

```DAX
Average Order Value =
DIVIDE(
    [Total Sales],
    [Total Orders]
)
```

```DAX
Average Rating =
AVERAGE(Customer_feedbacks[Rating])
```

> **Note:** The exact column names may differ depending on the final Power BI data model.

---

## 📊 Interactive Dashboard

The Power BI dashboard provides an interactive interface for exploring business performance.

### Dashboard Features

* KPI Cards
* Interactive Charts
* Slicers
* Filters
* Bar Charts
* Line Charts
* Donut Charts
* Tables
* Matrix Visuals
* Drill-down analysis
* Cross-filtering
* Time-based analysis
* Category-level analysis
* Product-level analysis

Users can start with a high-level overview and then drill into specific areas such as products, customers, orders, delivery, inventory, and customer feedback.

---

## 📈 Key Performance Indicators

The dashboard is designed to provide visibility into important business KPIs such as:

| KPI                       | Business Purpose                                |
| ------------------------- | ----------------------------------------------- |
| **Total Sales**           | Measures overall sales performance              |
| **Total Orders**          | Measures order volume                           |
| **Total Customers**       | Measures customer base                          |
| **Total Products**        | Provides product-level business coverage        |
| **Average Order Value**   | Helps understand average transaction value      |
| **Average Rating**        | Provides an indication of customer satisfaction |
| **Quantity Sold**         | Measures product demand                         |
| **Category Sales**        | Compares performance across categories          |
| **Product Sales**         | Identifies product-level contribution           |
| **Delivery Performance**  | Supports operational analysis                   |
| **Inventory Performance** | Supports stock monitoring                       |

---

## 🔍 Business Analysis

### 💰 Sales Analysis

The sales analysis focuses on understanding:

* Overall sales performance
* Sales trends over time
* Sales by product
* Sales by category
* High-performing periods
* Product contribution to overall sales

This analysis helps identify changes in demand and business performance.

---

### 📦 Order Analysis

Order analysis provides visibility into:

* Total order volume
* Order trends
* Order patterns
* Order status
* Period-wise order performance
* Product-level order activity

---

### 🛍️ Product Analysis

Product analysis helps identify:

* High-performing products
* Low-performing products
* Product contribution
* Category performance
* Product demand patterns
* Products requiring further attention

---

### 👥 Customer Analysis

Customer analysis focuses on understanding:

* Customer purchasing behavior
* Customer contribution
* Customer trends
* Customer segmentation
* Customer feedback
* Customer satisfaction

---

### 🚚 Delivery & Operations Analysis

Delivery analysis helps monitor:

* Delivery performance
* Fulfillment activity
* Operational trends
* Delivery patterns
* Potential operational bottlenecks
* Performance across different periods or locations

---

### 📦 Inventory Analysis

Inventory analysis helps understand:

* Product availability
* Inventory levels
* Stock-related trends
* Product demand versus inventory
* Products requiring inventory attention

This can support better inventory planning and operational decision-making.

---

### 📢 Marketing Analysis

Marketing analysis provides visibility into:

* Marketing activities
* Campaign performance
* Marketing trends
* Marketing and sales relationships
* Business response to marketing activity

---

### ⭐ Customer Feedback & Rating Analysis

Customer feedback analysis focuses on:

* Rating distribution
* Customer feedback
* Satisfaction trends
* Product/customer experience
* Areas that may require improvement

---

## 💡 Business Insights

The dashboard can help business users identify meaningful patterns across multiple areas.

### Sales Insights

* Understand changes in sales performance over time.
* Identify products and categories contributing to sales.
* Compare sales across different periods.
* Identify changes in demand.

### Customer Insights

* Understand customer purchasing patterns.
* Analyze customer contribution.
* Monitor customer satisfaction.
* Identify rating and feedback trends.

### Product Insights

* Identify products with strong sales performance.
* Compare products within categories.
* Understand product demand.
* Identify products that may require further investigation.

### Operational Insights

* Monitor delivery performance.
* Analyze fulfillment trends.
* Identify potential operational bottlenecks.
* Monitor inventory-related trends.

### Marketing Insights

* Compare marketing activity with business performance.
* Analyze campaign-related trends.
* Understand how marketing activity can be evaluated alongside sales.

---

## 🎯 Key Business Questions

The dashboard is designed to help answer questions such as:

1. What is the overall sales performance?
2. How many orders are being generated?
3. Which products contribute the most to sales?
4. Which categories perform the best?
5. How does sales performance change over time?
6. What are the major customer purchasing patterns?
7. Which products require inventory attention?
8. How is delivery performance changing?
9. What are the customer rating and feedback trends?
10. How can marketing performance be analyzed alongside sales?
11. Which areas may require further operational investigation?
12. How can historical business data support better decision-making?

---

## 🖼️ Dashboard Preview

Add screenshots of your Power BI dashboard below.

```markdown
## Dashboard Preview

### Executive Overview

![Executive Overview](Dashboard/executive_overview.png)

### Sales Analysis

![Sales Analysis](Dashboard/sales_analysis.png)

### Customer Analysis

![Customer Analysis](Dashboard/customer_analysis.png)

### Operations Analysis

![Operations Analysis](Dashboard/operations_analysis.png)
```

> Replace the image paths with the actual names of your screenshot files.

---

## 📁 Project Structure

A recommended GitHub repository structure is:

```text
Blinkit-PowerBI-Analytics/
│
├── README.md
│
├── Power_BI_project.pbix
│
├── Dashboard/
│   ├── executive_overview.png
│   ├── sales_analysis.png
│   ├── customer_analysis.png
│   └── operations_analysis.png
│
└── Data/
    └── source_data/
```

If the source dataset cannot be publicly shared, the `Data` folder can be omitted.

---

## 🚀 How to Use the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/blinkit-powerbi-dashboard.git
```

### 2. Open the Power BI File

Open:

```text
Power_BI_project.pbix
```

using **Microsoft Power BI Desktop**.

### 3. Refresh the Data

If the source data is available:

1. Open the PBIX file.
2. Go to **Home → Refresh**.
3. Verify the data source.
4. Check the relationships in the data model.
5. Interact with the dashboard using filters and slicers.

---

## 🎓 Skills Demonstrated

This project demonstrates practical experience in:

### Power BI

* Dashboard development
* Interactive reporting
* Data visualization
* KPI development
* Slicers and filters
* Drill-down analysis

### DAX

* Measure creation
* Aggregation
* Calculated metrics
* KPI calculations
* Analytical calculations

### Power Query

* Data cleaning
* Data transformation
* Data type management
* Data preparation

### Data Modeling

* Relational data modeling
* Table relationships
* Business entity modeling
* Analytical model design

### Data Analytics

* Sales analysis
* Customer analysis
* Product analysis
* Operations analysis
* Inventory analysis
* Marketing analysis
* Customer satisfaction analysis

---

## 🧠 Interview Discussion Points

This project demonstrates an end-to-end approach to solving a Business Intelligence problem.

### Problem

Business data was distributed across multiple areas including orders, customers, products, delivery, inventory, marketing, and feedback.

### Approach

The data was prepared, transformed, modeled, and analyzed in Power BI.

The process included:

```text
Data Collection
      ↓
Data Cleaning
      ↓
Data Transformation
      ↓
Data Modeling
      ↓
DAX Measures
      ↓
Dashboard Development
      ↓
Business Analysis
```

### Solution

An interactive Power BI dashboard was developed to provide a centralized view of business performance and allow users to explore different business dimensions.

### Key Learning

Through this project, I developed practical experience in:

* Understanding business requirements
* Preparing business data
* Designing a Power BI data model
* Creating DAX measures
* Building interactive dashboards
* Analyzing business KPIs
* Translating data into business insights
* Communicating analytical findings visually

---

## 📌 Project Highlights

### Business Areas

* 📈 Sales Analysis
* 📦 Order Analysis
* 🛍️ Product Analysis
* 👥 Customer Analysis
* 🚚 Delivery Analysis
* 📦 Inventory Analysis
* 📢 Marketing Analysis
* ⭐ Customer Feedback & Rating Analysis

### Technical Areas

* Microsoft Power BI
* Power Query
* DAX
* Data Modeling
* Data Visualization
* Business Intelligence
* Interactive Dashboard Development

---

## 🔮 Future Improvements

The project can be further enhanced with:

* Automated data refresh
* Power BI Service deployment
* Live database connectivity
* Advanced customer segmentation
* Sales forecasting
* Demand forecasting
* Predictive inventory analysis
* Customer Lifetime Value analysis
* Marketing ROI analysis
* Automated KPI alerts
* Advanced time-series analysis

---

## 📚 Project Outcome

The final solution demonstrates how raw business data can be transformed into an interactive Business Intelligence dashboard.

The complete workflow is:

```text
Raw Business Data
       ↓
Data Cleaning
       ↓
Data Transformation
       ↓
Data Modeling
       ↓
DAX Measures
       ↓
Interactive Dashboard
       ↓
Business Insights
       ↓
Data-Driven Decision Making
```

The project provides a centralized analytical view of **sales, orders, customers, products, delivery, inventory, marketing, and customer feedback**, allowing users to explore business performance through interactive Power BI visualizations.

---

## 👩‍💻 Author

**Your Name**

Aspiring Data Analyst | Business Intelligence | Power BI

### Technical Skills

`Power BI` • `DAX` • `Power Query` • `SQL` • `Excel` • `Data Analysis` • `Data Visualization`

---

## ⭐ Project Purpose

This project was developed as a practical **Business Intelligence portfolio project** to demonstrate the ability to transform raw business data into an interactive analytical solution using Power BI.

The project focuses not only on dashboard development, but also on:

* Understanding business requirements
* Preparing and transforming data
* Building a structured data model
* Developing analytical measures
* Creating meaningful KPIs
* Designing interactive visualizations
* Extracting business insights
* Communicating data effectively

---

## 📄 License

This project is intended for **educational and portfolio purposes**.

If the underlying dataset belongs to a third party, all rights related to the original dataset remain with its respective owner.

---

## ⭐ If You Found This Project Useful

Feel free to ⭐ the repository and explore the Power BI project.
