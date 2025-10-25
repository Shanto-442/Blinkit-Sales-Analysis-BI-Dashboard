# 🟡 Blinkit Sales Performance Dashboard

## 📊 Overview
This interactive **Power BI dashboard** presents a detailed overview of **Blinkit’s** sales performance across different outlets, item types, and regions.  
It enables stakeholders to monitor sales trends, outlet efficiency, and product category performance — all in one visual interface.

---

## 🚀 Key Features
- 💰 **Total Sales:** $1.20M overall revenue performance  
- 💵 **Average Sales:** $140.99 per transaction  
- 📦 **Number of Items:** 8,523 unique products  
- ⭐ **Average Rating:** 3.92 customer satisfaction score  

### Visual Insights Include:
- **Outlet Establishment Trend:** Line chart showing sales growth (2012–2022) with a peak in 2018 ($205K).  
- **Item Type Analysis:** Bar chart visualizing top-performing categories — Fruits, Snacks, Household, Dairy, etc.  
- **Fat Content Breakdown:** Comparison of Regular vs. Low-Fat products across outlet tiers.  
- **Outlet Size Performance:** Donut chart segmenting High, Medium, and Small outlets.  
- **Outlet Location Comparison:** Tier-based performance (Tier 1–3) highlighting sales and visibility metrics.  
- **Outlet Type Table:** Comprehensive metrics table with:
  - Total Sales  
  - Average Sales  
  - No. of Items  
  - Average Ratings  
  - Item Visibility

---
## 🧮 Data Analysis Process

### 1. **Data Collection**
- The raw dataset was imported from Blinkit’s internal sales records containing:
  - Outlet information (size, location, establishment year)  
  - Product details (item type, fat content, visibility)  
  - Performance metrics (sales, ratings, item count)

### 2. **Data Cleaning & Transformation (Power Query)**
- Handled **missing and null values** using conditional replacement.  
- Standardized inconsistent outlet names and product types.  
- Converted data types (e.g., text → numeric for sales values).  
- Created new calculated columns for:
  - `Average Sales = Total Sales / No. of Items`
  - `Item Visibility Score`  
  - Categorization of outlets (Tier 1, 2, 3)

### 3. **Data Modeling**
- Built **relationships** between datasets:
  - Outlet Table ↔ Item Table  
  - Sales Table ↔ Outlet Dimension  
- Defined primary keys and lookup tables for efficient filtering.  
- Applied **DAX measures** for:
  - Total Sales (`SUM(Sales[SalesAmount])`)
  - Average Rating (`AVERAGE(Rating)`)
  - Average Sales (`DIVIDE(SUM(Sales[SalesAmount]), COUNT(Items[ItemID]))`)

### 4. **Data Visualization (Dashboard Design)**
- Created multiple **interactive visuals** in Power BI:
  - **Cards** for KPIs (Total Sales, Avg Sales, No. of Items, Avg Rating)  
  - **Line Chart** for outlet establishment trend  
  - **Bar Chart** for item types  
  - **Donut Charts** for outlet size and fat content  
  - **Table Visual** for detailed performance metrics  
- Applied **slicers** (filters) for Outlet Size, Location, and Item Type.  
- Used consistent **color coding** (yellow, green, white) matching Blinkit’s brand identity.

### 5. **Insights & Interpretation**
- Identified high-performing outlets (Tier 3, Supermarket Type 1).  
- Observed a strong correlation between outlet establishment year and revenue.  
- Found customer preference trends for low-fat and snack items.  
- Noted item visibility impact on sales consistency.

### 6. **Dashboard Optimization**
- Improved usability with:
  - Tooltips for deeper insight on hover.  
  - Clean layout for visual hierarchy.  
  - Uniform formatting for KPIs and labels.  

---

## 🧩 Interactive Filters
Dynamic filters allow customized analysis by:
- **Outlet Location**  
- **Outlet Size**  
- **Item Type**

These filters make it easy to drill down into specific outlet types or product categories.

---

## 📈 Insights Summary
- 🏪 **Tier 3 outlets** lead with **$472.13K** in total sales.  
- 🛒 **Supermarket Type 1** generates the highest revenue (**$787.55K**).  
- 🧈 **Low-fat items** maintain strong average sales comparable to regular ones.  
- 📉 Sales peaked in **2018**, showing significant year-over-year fluctuations.

---

## 🛠️ Tools & Technologies
- **Platform:** Power BI  
- **Dataset:** Blinkit Sales Dataset  
- **Metrics:** Total Sales, Average Sales, No. of Items, Avg. Rating, Visibility  
- **Purpose:** To evaluate outlet performance, product category trends, and customer satisfaction.

---

## 🎯 Business Purpose
This dashboard helps:
- **Management** — to monitor outlet and product performance.  
- **Marketing Analysts** — to identify top-performing categories.  
- **Operations Teams** — to make data-driven decisions for improving sales, stock levels, and strategy.

---

## 📂 File Information
**File Name:** `Blinkit_Sales_Dashboard.pbix`  
**Created With:** Microsoft Power BI  
**Last Updated:** October 2025

---

## 🧠 Author
Developed by **Shanto Mia**  
📍 University of Dhaka | Finance Graduate & Data Analyst  
📧 For queries: shantomia442@gmail.com

---

⭐ _If you find this project useful, consider giving it a star on GitHub!_

Image Preview of the Deshboard: https://github.com/Shanto-442/Blinkit-Sales-Analysis-BI-Dashboard/blob/main/Image%20of%20Blinkit%20Sales%20Dashboard.png
