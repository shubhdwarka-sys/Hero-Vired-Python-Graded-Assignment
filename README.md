# 🚗 Used Car Price Analysis — EDA Project

**Hero Vired | Python Graded Assignment**
**Author:** Subhash Adhikari | **Batch:** 9B_12349

---

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a real-world used car listings dataset using Python and Pandas. The analysis covers data cleaning, querying, and visualization to extract meaningful business insights from 5.5 lakh+ car records.

---

## 📂 Files in this Repository

| File | Description |
|------|-------------|
| `Car Prices Assignment Final.ipynb` | Main Jupyter Notebook — all tasks |
| `car_prices.csv` | Dataset — used car listings |
| `README.md` | Project documentation |

---

## 🗂️ Dataset Info

| Attribute | Details |
|-----------|---------|
| Source | Used Car Listings (Real-World) |
| Records | 5,58,837 rows |
| Columns | 16 (year, make, model, condition, odometer, sellingprice, state, color, etc.) |

---

## ✅ Tasks Completed

### Section 1 — Data Ingestion & Quality Profiling
- Loaded dataset and inspected first 5 rows
- Checked shape, column names, data types
- Identified and visualized null values (bar chart)
- Resolved nulls: median for numeric, mode for categorical
- Removed duplicate records

### Section 2 — DataFrame Queries (2.1 to 2.12)
- Average, Min, Max selling price
- Unique colors, brands, models
- Cars priced above $165,000
- Top 5 most frequently sold models
- Average price by brand, interior type
- Highest odometer per year
- New column: Car Age (2025 - year)
- Filtered by condition ≥ 48 AND odometer > 90,000
- State with highest prices for newer cars (year > 2013)
- Best value-for-money brands in excellent condition (top 20%)

### Section 3 — Data Visualization & Insights
- Correlation heatmap of numerical features
- Average selling price by year (Bar chart)
- Average selling price by odometer (Scatter plot)
- Number of cars sold per state (Bar chart)
- Avg price by condition score range (size 5)
- Count of cars by condition range (size 10)
- Box plot by color — with & without outliers (IQR per color)

---

## 🔧 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 💡 Key Insights

- **sellingprice & mmr** are strongly correlated (~0.98)
- **Newer cars (2013–2015)** command the highest average prices
- **Higher mileage = lower price** — clear downward trend
- **FL, CA, PA** are top 3 states by car sales volume
- **OH (Ohio)** has the highest avg price for newer cars
- **Isuzu & Honda** offer best value in excellent condition
- **Color is NOT a strong price driver** — minimal variation across colors

---

## ▶️ How to Run

1. Clone this repository
```bash
git clone https://github.com/YOUR_USERNAME/car-price-eda.git
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn
```

3. Open notebook in VS Code or Jupyter
```bash
jupyter notebook "Car Prices Assignment Final.ipynb"
```

---

## 📊 Sample Visualizations

- Correlation Heatmap
- Price by Year (Bar)
- Price by Odometer (Scatter)
- Box Plot by Color (IQR cleaned)

---

*Submitted as part of Hero Vired CPDA Program — Python Graded Assignment*
