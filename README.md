# AhlyBank-Power BI
<img width="965" height="585" alt="Screenshot 2026-01-01 231152" src="https://github.com/user-attachments/assets/8ef4d2d7-a07d-45d2-8f12-df00f3d5958c" />
<img width="971" height="589" alt="Screenshot 2026-01-01 231238" src="https://github.com/user-attachments/assets/849eff4c-3eca-4c5c-a57c-41b64faaa0ab" />
<img width="968" height="585" alt="Screenshot 2026-01-01 231406" src="https://github.com/user-attachments/assets/75721d28-df7a-45d6-9c26-2b64423c9556" />
<img width="1086" height="572" alt="Screenshot 2026-01-01 231634" src="https://github.com/user-attachments/assets/11a359d3-254f-4d29-9fc4-e1528e61d1a8" />


## 📊 Project Overview

This is my first Power BI project for banking analytics: a comprehensive analytical dashboard for **Ahly Bank** data.

The goal was to transform raw banking data (**Transactions, Loans, Accounts, Support Calls, Customers, Cards**) into actionable insights to understand **customer behavior, transaction patterns, loan portfolios, and support performance**.

This project helped me learn Power BI with real-world banking data, including **data cleaning, modeling, DAX, and dashboard design**.

---

## ✨ Key Features

- 📈 Interactive dashboard covering **Customer Engagement, Transactions & Products, Loans Portfolio, and Support & Service Quality**
- 👥 Analysis of **customer activity (Active vs Inactive)** and engagement trends
- 📅 Year-over-Year comparison of Transactions and Loans
- 🔍 Insights into top customers, account types, and business segments
- 📞 Performance tracking of **Support Calls** and Resolution Rate
- 🎯 Dynamic filtering across all visuals using a **Calendar Table**

---

## 💡 Key Insights

| Metric | Value | Notes |
|--------|-------|-------|
| **Active Customers** | 60% | ~2,000 inactive customers → re-engagement opportunity |
| **Business Accounts** | 35% | Potential for targeted B2B offers |
| **Support Resolution Rate** | 49% | Goal: >75% (needs improvement) |
| **Top Loan Type** | Car Loans | Focus area for marketing |
| **Transaction Trends** | Drop in 2025 | Requires further investigation after 2023-2024 growth |

---

## 🛠️ Project Steps

### 1️⃣ Data Cleaning
- Handled nulls and duplicates
- Corrected unusual date formats
- Standardized columns across multiple tables

### 2️⃣ Data Modeling
- Created **Star Schema** linking **Transactions** as Fact table to **Customers, Accounts, Loans, SupportCalls, Cards**
- **Calendar Table** linked to Transactions with relationships propagated through Customers
- Managed **Active/Inactive context using DAX (USERELATIONSHIP)** for correct filtering

### 3️⃣ DAX Measures
- Total Transactions Amount with **USERELATIONSHIP**
- Average Loan Duration (Months/Years)
- Active vs Inactive Customers
- Support Call Resolution Rate
- Dynamic KPIs for dashboard visuals

### 4️⃣ Visualization
Designed 4 main dashboard pages:
- **Overview:** Key metrics and KPIs
- **Customer Insights:** Engagement, Active vs Inactive
- **Transactions & Loans:** Trends and top customers
- **Support & Service Quality:** Resolution rates and improvement opportunities

---

## 📚 Lessons Learned

- Handling **complex relationships** between multiple banking tables
- Building a **strong and efficient data model** for financial datasets
- Using **DAX to manage context** (Active/Inactive, USERELATIONSHIP)
- Importance of **Calendar Table and filter propagation**

### 🏦 Banking vs E-commerce Insight

| E-commerce | Banking |
|------------|---------|
| Linking Calendar to Sales table is usually enough | Multiple tables with different dates require complex modeling |
| Filters propagate automatically | Requires linking Calendar to **Fact table (Transactions)** |
| Simple relationship management | Managing relationships to **Customers** and related tables |
| - | Using DAX measures like `USERELATIONSHIP` for Active/Inactive context |

> **Key Takeaway:** This ensures **filters on Calendar work correctly across all visuals**, which was a critical challenge I learned to handle in this banking project.

---

## 🚀 How to Use

1. Download the `.pbix` file from this repository
2. Open with Power BI Desktop
3. Explore the interactive dashboards
4. Use slicers and filters to drill down into specific insights

---

## 📧 Contact

Feel free to reach out for questions or collaboration opportunities!

---

## 📝 License

This project is for educational and portfolio purposes.
