# Aurora Banking Performance Dashboard

## Overview

Aurora Banking Performance Dashboard is a Power BI project designed to analyze banking transaction performance, customer value, merchant behavior, and risk signals. The dashboard helps identify where Aurora Banking is performing well, which customer segments drive the most value, and which areas require attention due to transaction failures or risk exposure.

The project is built around four main analytical views:

1. **Overview** — overall Aurora performance and transaction trends.
2. **Customer Segment** — customer value, activity, credit score, and age-based insights.
3. **Merchant** — channel performance, merchant category contribution, and spending behavior.
4. **Risk** — failed transaction behavior, insufficient balance exposure, and high-risk segments.

A simple **Insight Page** is also included to summarize the most important business findings in a clear, text-based format.

---

## Key Business Questions

This dashboard is designed to answer the following questions:

- How is Aurora Banking’s overall transaction performance trending?
- Which customer segments generate the most value and growth potential?
- Where does transaction performance vary across channels and merchants?
- Which customer or merchant segments show higher risk and require attention?
- What are the main drivers behind transaction success, value, and failure?

---

## Key Insights

- Aurora Banking shows strong overall performance with a high transaction success rate of approximately **98.26%**.
- Total transaction volume is around **157K transactions**, with approximately **$6.707M** in Net Successful Transaction Value.
- Transaction value and volume show a noticeable decline toward the end of the year, especially around **November and December**.
- **Debit cards** are the main transaction driver, contributing the largest share of transaction value.
- Customers in the **Good credit score band** generate the highest value, making them a key segment for retention and growth.
- Mature customer groups, especially **45–54** and **55+**, contribute strongly to transaction value.
- Spending is concentrated in essential merchant categories such as **Food & Grocery**, **Retail & Consumer Goods**, **Financial & Insurance**, and **Utilities & Telecom**.
- Failed transactions remain relatively low but still represent a value leakage opportunity, with insufficient balance being one of the main risk drivers.

---

## Dataset

The dashboard is built using the following datasets:

| File | Description |
|---|---|
| `transactions_data.xlsx` | Transaction-level data including transaction amount, status, channel, merchant, and card information. |
| `users_data.xlsx` | Customer demographic and profile information. |
| `cards_data.xlsx` | Card-level information such as card type and card brand. |
| `mcc_codes.xlsx` | Merchant category code reference data. |

These files are used to build relationships, calculate KPIs, and create dashboard visuals in Power BI.

---

## Dashboard Pages

### 1. Overview

The Overview page summarizes total customers, active customers, total transactions, Net Successful Transaction Value, success rate, card type contribution, customer mix, merchant category performance, and monthly performance trends.

### 2. Customer Segment

The Customer Segment page focuses on identifying which customer groups drive the most value. It analyzes customer value by age band, credit score band, income, activity level, and transaction frequency.

### 3. Merchant

The Merchant page analyzes transaction performance across merchant categories, merchant groups, channels, weekdays, and time buckets. It helps identify where customers spend the most and which merchant areas contribute most to transaction value.

### 4. Risk

The Risk page highlights failed transaction behavior, insufficient balance exposure, failed transaction value, high-risk customer groups, and merchant groups with higher risk signals.

### 5. Insight Page

The Insight page provides a simple executive summary of the most important findings, focusing on performance, value drivers, merchant behavior, and risk areas.

---

## Tools Used

- **Power BI Desktop** — dashboard design, data modeling, DAX measures, and visualization.
- **Microsoft Excel** — source data files.
- **Power Query** — data cleaning, transformation, and preparation.
- **DAX** — KPI calculations and business measures.

---

## Suggested Repository Structure

```text
Aurora-Banking-Dashboard/
│
├── README.md
├── Aurora_Banking_Dashboard.pbix
│
├── data/
│   ├── transactions_data.xlsx
│   ├── users_data.xlsx
│   ├── cards_data.xlsx
│   └── mcc_codes.xlsx
│
├── images/
│   ├── overview.png
│   ├── customer_segment.png
│   ├── merchant.png
│   ├── risk.png
│   └── insight.png
│
└── docs/
    └── business_insights.md
```

---

## How to Open the Project

1. Clone or download this repository.
2. Open `Aurora_Banking_Dashboard.pbix` using Power BI Desktop.
3. Make sure the Excel source files are stored in the `data/` folder.
4. If needed, update the data source path in Power Query.
5. Refresh the dashboard to load the latest data.

---

## How to Push This Project to GitHub

### 1. Create a new repository on GitHub

Create a new repository, for example:

```text
Aurora-Banking-Dashboard
```

### 2. Open the project folder in terminal

```bash
cd path/to/Aurora-Banking-Dashboard
```

### 3. Initialize Git

```bash
git init
```

### 4. Add project files

```bash
git add .
```

### 5. Commit the files

```bash
git commit -m "Initial commit: Aurora Banking Power BI dashboard"
```

### 6. Connect to your GitHub repository

Replace the URL below with your own GitHub repository URL:

```bash
git remote add origin https://github.com/your-username/Aurora-Banking-Dashboard.git
```

### 7. Push to GitHub

```bash
git branch -M main
git push -u origin main
```

---

## Notes

- If the `.pbix` file is large, consider using **Git LFS**.
- Avoid uploading sensitive or private customer data to a public repository.
- If this project is for portfolio use, use anonymized or sample data only.
- Add dashboard screenshots to the `images/` folder so visitors can preview the project without opening Power BI.

---

## Author

Created as part of a Power BI analytics project for Aurora Banking performance, customer segmentation, merchant performance, and transaction risk analysis.
