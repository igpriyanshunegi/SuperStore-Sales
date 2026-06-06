# 🛒 SuperStore Sales Analysis

> An end-to-end data analysis project covering **5,900+ orders** across the United States (2019–2020), combining Python-based EDA, interactive visualizations, and a Power BI dashboard.

---

## 📊 Dashboard Preview


📌 ![Power BI Dashboard](https://your-screenshot-link-here.com/dashboard.png)
📌 ![Power BI Dashboard](https://your-screenshot-link-here.com/dashboard.png)

---

## 📁 Project Structure

```
SuperStore-Sales/
│
├── SuperStore_Sales_Dataset.csv       # Raw sales dataset (2019–2020)
├── SuperStore_Sales_Analysis.ipynb    # Python EDA notebook
├── supersaledashboard.pbix            # Power BI interactive dashboard
└── README.md
```

---

## 🗂️ Dataset Overview

**File:** `SuperStore_Sales_Dataset.csv`

| Property | Details |
|---|---|
| Total Records | 5,901 orders |
| Time Period | January 2019 – December 2020 |
| Geographic Coverage | United States (4 regions) |
| Total Columns | 23 |

### Key Columns

| Column | Description |
|---|---|
| `Order ID` | Unique order identifier |
| `Order Date` / `Ship Date` | Order and shipment timestamps |
| `Ship Mode` | Standard Class, First Class, Second Class, Same Day |
| `Customer Name` / `Segment` | Customer info — Consumer, Corporate, Home Office |
| `Region` / `State` / `City` | Geographic dimensions |
| `Category` / `Sub-Category` | Product hierarchy — Furniture, Technology, Office Supplies |
| `Sales` / `Profit` / `Quantity` | Core financial metrics |
| `Payment Mode` | Online, Cards, COD |
| `Returns` | Return flag per order |

---

## 🐍 Python EDA — Notebook Highlights

**File:** `SuperStore_Sales_Analysis.ipynb`

**Libraries Used:** `pandas` · `numpy` · `matplotlib` · `seaborn`

### Analysis Performed

**1. Data Cleaning & Preprocessing**
- Parsed `Order Date` and `Ship Date` as datetime objects
- Dropped irrelevant columns (`ind1`, `ind2`)
- Filled missing return values with `0`
- Checked for and removed duplicate records
- Engineered `Year` and `Month` features from order dates

**2. KPI Summary**
- Total Sales, Total Profit, and Unique Order Count

**3. Sales & Profit Analysis**
- Sales and profit breakdown by **Category**
- Top 10 **States** by sales
- Top 10 **Products** by revenue
- **Regional** sales distribution (pie chart)
- **Customer segment** comparison

**4. Time-Series Analysis**
- Monthly sales trend over the full two-year period

**5. Payment Behaviour**
- Sales volume split across Online, Cards, and COD

**6. Correlation & Returns**
- Scatter plot of Sales vs. Profit
- Correlation heatmap (Sales · Quantity · Profit)
- Return rate calculation

---

## 📊 Power BI Dashboard

**File:** `supersaledashboard.pbix`

The Power BI dashboard provides an interactive view of the same dataset with slicers, drill-throughs, and dynamic visuals. Open the file in **Power BI Desktop** to explore.

**What's inside:**
- KPI cards for total Sales, Profit, and Orders
- Time-series charts for monthly and yearly trends
- Category and sub-category performance visuals
- Region and state-level geographic breakdown
- Customer segment and payment mode analysis
- Return order tracking

---

## ⚙️ How to Run

### Python Notebook

**Prerequisites**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

**Steps**
```bash
# 1. Clone the repository
git clone https://github.com/igpriyanshunegi/SuperStore-Sales.git
cd SuperStore-Sales

# 2. Launch Jupyter
jupyter notebook SuperStore_Sales_Analysis.ipynb
```

Make sure `SuperStore_Sales_Dataset.csv` is in the **same directory** as the notebook.

### Power BI Dashboard

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Open `supersaledashboard.pbix`
3. If prompted, update the data source path to point to `SuperStore_Sales_Dataset.csv` on your machine

---

## 🔍 Key Insights

- 📦 **Technology** drives the highest sales, while **Office Supplies** leads in order volume
- 🌎 The **West** and **East** regions account for the majority of revenue
- 💳 **Online** is the dominant payment mode
- 📈 Sales peak toward **Q4** each year, following typical retail seasonality
- 📉 Some sub-categories show negative profit despite positive sales — a key area for business review

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)

---

## 👤 Author

**Priyanshu Negi**
[GitHub](https://github.com/igpriyanshunegi) · [LinkedIn](https://linkedin.com/in/igpriyanshunegi)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
