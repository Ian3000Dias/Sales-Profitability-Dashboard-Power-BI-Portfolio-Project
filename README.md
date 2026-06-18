# 📊 Sales & Profitability Dashboard — Power BI Portfolio Project

An end-to-end Power BI project analysing sales performance and profitability across products and accounts. Built to demonstrate real-world data modelling, DAX, and dashboard design skills.

---

## 🗂️ Dataset Overview

The project uses a star schema with one fact table and two dimension tables:

| Table | Type | Description |
|---|---|---|
| **Fact Table** | Fact | Core transactional data — Product ID, Account ID, Sales, Prices, and Costs |
| **Accounts** | Dimension | Additional account-level details (customer/region info) |
| **Plant Hierarchy** | Dimension | Product hierarchy and classification details |

---

## 🔧 Technical Walkthrough

### 1. Loading Data
- Connected to source data via **Get Data → Excel Workbook**
- Used **Power Query (Transform & Load)** to:
  - Validate and correct data types
  - Remove duplicates where necessary
  - Standardise table naming conventions

### 2. Data Modelling
- Built a **star schema** by defining relationships between the fact table and both dimension tables
- Created **virtual tables** using DAX via the Modelling tab (`New Table`)
- Used **Enter Data** for lookup/reference tables where needed
- Organised related columns into **display folders** (Model View → Display Folder) for a clean, navigable field list

### 3. DAX Measures
Custom measures were created by right-clicking tables in the Data pane. Key measure categories include:

- **Sales measures** — total revenue, quantity sold
- **Cost & profitability measures** — gross profit, profit margin %
- **Comparison measures** — YoY or period-over-period variance

### 4. Report Design
The dashboard includes a mix of visual types:

- **Cards & KPIs** — high-level headline metrics (revenue, profit, margin %)
- **Bar / Column & Line charts** — trend analysis and category breakdowns
- **Tables** — granular account/product-level detail
- **Maps & Slicers** — geographic filtering and interactive drill-downs
- **Conditional formatting** — colour-coded indicators for metrics trending up or down, applied to key value columns for instant insight

---

## 📁 Project Structure

```
├── PlantCo_Dashboard.pbix    # Main Power BI report file
├── Data/
│   └── PlantCo_Data.xlsx     # Source Excel dataset
└── README.md
```

---

## 💡 Key Skills Demonstrated

- Power Query data transformation and cleaning
- Star schema data modelling in Power BI
- DAX measure creation (calculated columns, virtual tables, aggregations)
- Conditional formatting for business KPIs
- Dashboard layout and UX design principles

---

## 📺 Project Credit

This project was built by following the guided series by **Mo Chen** on YouTube:
[Power BI Full Project Playlist](https://www.youtube.com/watch?v=BLxW9ZSuuVI&list=PLodYDTuHA29aWHT5lVILqoI_cZWBXloHr&index=1)

All implementation, notes, and documentation are my own.

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `PlantCo_Dashboard.pbix` in **Power BI Desktop**
3. If prompted, re-point the data source to the `Data/` folder
4. Explore the report pages and interact with slicers/filters

---

## 👤 Author

**[Ian Dias]**
[LinkedIn]([https://www.linkedin.com/in/iandias20/]) · [GitHub]([https://github.com/Ian3000Dias])
