# 🛒 Blinkit Sales & Operations Analytics Dashboard | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Analytics-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data-Analytics-blue?style=for-the-badge)
![SQL](https://img.shields.io/badge/SQL-Data%20Preparation-orange?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Project-black?style=for-the-badge&logo=github)

## 📌 Project Overview

This project is an end-to-end **Blinkit Sales & Operations Analytics Dashboard** developed using **Microsoft Power BI**.

The objective of the project is to transform business data related to orders, customers, products, delivery, inventory, marketing, ratings, and feedback into an interactive analytical dashboard.

The dashboard is designed to help business stakeholders understand sales performance, customer behavior, product performance, operational efficiency, inventory trends, and customer satisfaction through data-driven insights.

---

## 🎯 Business Objective

The primary objective of this project is to build a centralized Business Intelligence solution that can answer questions such as:

- How are sales and order volumes performing?
- Which products and categories contribute most to business performance?
- What customer segments generate the highest business value?
- How does delivery performance vary across different locations or periods?
- Which products require greater inventory attention?
- What are the major customer feedback and rating trends?
- How can marketing performance be analyzed alongside sales?
- Which areas require operational improvement?

The dashboard converts raw business data into meaningful visual insights that can support faster and more informed decision-making.

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **Microsoft Power BI** | Data modeling, DAX, visualization and dashboard development |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures, calculated columns and analytical calculations |
| **Data Modeling** | Relationships between business entities |
| **SQL** | Data querying and analytical preparation |
| **Excel / CSV** | Source data handling |
| **GitHub** | Project documentation and portfolio presentation |

---

## 🗂️ Data Model

The Power BI project uses a relational data model consisting of multiple business entities.

### Main Tables

- **Orders**
  - Order-level transaction information
  - Order dates
  - Customer references
  - Order status and related attributes

- **Order_item**
  - Individual items associated with orders
  - Product-level transaction information
  - Quantity and order-item attributes

- **Products**
  - Product information
  - Product/category attributes
  - Product-level analysis

- **Customer**
  - Customer information
  - Customer-related attributes
  - Customer segmentation and analysis

- **Customer_feedbacks**
  - Customer feedback information
  - Feedback and satisfaction analysis

- **Delivery**
  - Delivery-related information
  - Operational and fulfillment analysis

- **Inventory**
  - Inventory-related information
  - Product availability and stock analysis

- **Marketing**
  - Marketing-related information
  - Campaign and marketing performance analysis

- **Master_Table**
  - Central/master business information used within the analytical model

- **Folder**
  - Supporting organizational/reference data

- **Category_Icon**
  - Category-related supporting information

- **Ratings_Icon**
  - Rating-related supporting information

---

## 🔄 Data Preparation Process

The data preparation process follows a typical Business Intelligence workflow:

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
