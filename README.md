# 🛒 E-Commerce Sales Analytics Dashboard | Tableau

## 📌 Project Overview

An interactive Tableau dashboard built using a multi-table Brazilian E-Commerce dataset to analyze sales performance, customer behavior, product trends, payment methods, and order status. The project integrates multiple related datasets using Tableau Relationships and leverages calculated fields, filters, KPIs, and interactive visualizations to support business decision-making.

---

# 📊 Dashboard 1 – Executive Sales Overview

Provides a high-level overview of overall sales performance and key business metrics.

### Analysis Includes

- 💰 Total Sales
- 📦 Total Orders
- 👥 Unique Customers
- ⭐ Average Review Score
- 📈 Profit Margin %
- 💵 Estimated Profit
- 📅 Monthly Sales Trend
- 🛍️ Top Product Categories (Treemap)
- 🚚 Order Status Distribution
- Interactive Filters (Month, Order Status, Sales Range)

---

# 👥 Dashboard 2 – Customer Insights

Provides detailed insights into customer purchasing behavior and payment preferences.

### Analysis Includes

- 👤 Top 10 Customers by Revenue
- 💳 Payment Method Distribution
- Customer Search Filter
- Payment Type Filter
- Interactive KPI Cards

---

# 📷 Dashboard Preview

### Dashboard 1 – Executive Sales Overview
- Executive KPI Cards
- Monthly Revenue Trend
- Product Category Performance
- Order Status Distribution

  <img width="1320" height="653" alt="Page 1" src="https://github.com/user-attachments/assets/a3d1e26a-e4c9-4eff-b887-db8bd7d91ba1" />


### Dashboard 2 – Customer Insights
- Top Customers by Revenue
- Payment Method Analysis
- Customer-Level Filtering

  <img width="1318" height="650" alt="Page 2" src="https://github.com/user-attachments/assets/9ae026a2-640e-4d38-a0d9-a171bbc0c4a1" />


---

# 💡 Key Insights

- 📌 Generated total sales of **₹15.84M** across **99,441 orders**.
- 📌 Served **96,096 unique customers** with an average review score of **4.09**.
- 📌 Nearly **97% of all orders were successfully delivered**.
- 📌 Credit Card was the most preferred payment method.
- 📌 Beauty, Home, and Lifestyle categories generated the highest sales.
- 📌 Monthly sales showed steady growth with seasonal fluctuations.

---

# 💼 Business Recommendations

- 📊 Monitor monthly sales trends to improve inventory planning.
- 💳 Optimize payment strategies based on customer preferences.
- 🚚 Reduce canceled and unavailable orders to improve customer satisfaction.
- 🎯 Focus marketing campaigns on high-performing product categories.
- 👥 Reward high-value customers through loyalty programs.
- 📈 Use interactive dashboards for faster, data-driven decision-making.

---

# ⭐ Tableau Features Used

- ✅ Multi-Table Data Modeling (Relationships)
- ✅ Calculated Fields
- ✅ Logical Calculations (IF, ELSEIF, AND, OR)
- ✅ Date Calculations
- ✅ Aggregate Calculations
- ✅ KPI Cards
- ✅ Interactive Filters
- ✅ Treemap
- ✅ Line Chart
- ✅ Pie Chart
- ✅ Horizontal Bar Chart
- ✅ Conditional Formatting
- ✅ Dynamic Tooltips
- ✅ Dashboard Actions

---

# 📊 Calculated Fields Used

### Total Sales
```tableau
SUM([Price] + [Freight Value])
```

### Total Orders
```tableau
COUNTD([Order ID])
```

### Unique Customers
```tableau
COUNTD([Customer Unique Id])
```

### Average Review
```tableau
AVG([Review Score])
```

### Profit Margin %
```tableau
SUM([Price]) / SUM([Payment Value])
```

### Estimated Profit
```tableau
SUM([Price]) * 0.95
```

### High Value Order
```tableau
IF [Price] >= 500 THEN
"High Value"
ELSE
"Regular"
END
```

### Successful Orders
```tableau
IF [Order Status] = "delivered" THEN
"Successful"
ELSE
"Unsuccessful"
END
```

### Month Name
```tableau
DATENAME('month',[Order Purchase Timestamp])
```

### Order Year
```tableau
YEAR([Order Purchase Timestamp])
```

### Weekend Orders
```tableau
IF DATEPART('weekday',[Order Purchase Timestamp]) IN (1,7)
THEN "Weekend"
ELSE "Weekday"
END
```

---

# 📊 Visualizations Used

- KPI Cards
- Monthly Sales Trend (Line Chart)
- Product Category Treemap
- Order Status Distribution (Horizontal Bar)
- Top 10 Customers by Revenue (Bar Chart)
- Payment Method Distribution (Pie Chart)

---

# 🛠️ Tech Stack

- 📊 Tableau Desktop
- 📁 CSV Dataset
- 🔗 Tableau Relationships
- 📈 Data Visualization
- 📊 Business Intelligence
- 📉 Data Analytics

---

# 🎯 Business Impact

This Tableau dashboard transforms raw e-commerce data into an interactive business intelligence solution. By combining multiple datasets, calculated metrics, and dynamic visualizations, it enables stakeholders to monitor sales performance, understand customer behavior, analyze payment preferences, and track order fulfillment efficiently. The dashboard supports data-driven decision-making through interactive filtering, KPI monitoring, and clear performance insights.

---

## 👩‍💻 Author

**Drashti Patel**

### 🔗 LinkedIn

https://www.linkedin.com/in/drashtipatel16/

### 💻 GitHub

https://github.com/Drashti0347

---

⭐ If you found this project helpful, consider giving it a **Star ⭐** on GitHub!

🤝 Let's connect and collaborate on **Tableau, SQL, Power BI, Data Analytics, Data Visualization, and Business Intelligence** projects.
