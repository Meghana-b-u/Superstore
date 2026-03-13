# 📊 Superstore Sales Analysis — Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A live interactive **Sales Analytics Dashboard** built in Power BI Desktop using the Superstore retail dataset.

---

## 📸 Dashboard Preview

![Superstore Analysis Dashboard](./dashboard-screenshot.png)

---

## 📁 Project Structure

```
superstore-powerbi-dashboard/
├── Live_project.pbix
├── train.csv
├── dashboard-screenshot.png
└── README.md
```

---

## 📋 Dataset

| Property | Details |
|---|---|
| **Source** | [Kaggle — Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) |
| **Rows** | 9,800 orders |
| **Columns** | 18 columns |
| **Date Range** | 2015 – 2018 |

### Columns Used

| Column | Description |
|---|---|
| Order ID | Unique order identifier |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Ship Mode | Standard / First / Second / Same Day |
| Segment | Consumer / Corporate / Home Office |
| Region | West / East / Central / South |
| Category | Furniture / Technology / Office Supplies |
| Sub-Category | Phones / Chairs / Storage etc. |
| Sales | Revenue per order |

---

## 📊 Dashboard Visuals

| Visual | Type | Fields |
|---|---|---|
| Total Sales | KPI Card | SUM(Sales) |
| Total Orders | KPI Card | DISTINCTCOUNT(Order ID) |
| Avg Order Value | KPI Card | Sales / Orders |
| Sales by Sub-Category | Bar Chart | Sub-Category, Sales |
| Sales by Category | Bar Chart | Category, Sales |
| Sales by Region | Donut Chart | Region, Sales |
| Sales by Segment | Pie Chart | Segment, Sales |
| Sales by Month | Line Chart | Month, Sales |
| Top Sub-Categories | Table | Sub-Category, Sales |
| Region Filter | Tile Slicer | Region |
| Category Filter | Tile Slicer | Category |
| Date Filter | Date Range Slicer | Order Date |

---

## 🧮 DAX Measures

```dax
Total Sales = SUM('train'[Sales])
```

```dax
Total Orders = DISTINCTCOUNT('train'[Order ID])
```

```dax
Avg Order Value = DIVIDE([Total Sales], [Total Orders])
```

---

## 🔑 Key Insights

- 📱 **Phones** are the top sub-category — ₹3.27M in sales
- 🌍 **West region** leads with 31.4% of total sales
- 👤 **Consumer segment** is 50.7% of all customers
- 💻 **Technology** is the highest selling category at ₹0.83M
- 🚚 **Standard Class** is the most used shipping mode
- 💰 Total revenue across all years: **₹19,90,893**

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard and visualization |
| Power Query | Data cleaning and transformation |
| DAX | Custom calculated measures |
| CSV from Kaggle | Source dataset |

---

## 🚀 How to Run This Project

**Step 1** — Clone this repository

```bash
git clone https://github.com/Meghana-b-u/superstore-powerbi-dashboard.git
```

**Step 2** — Open Power BI Desktop

```
Download free from https://powerbi.microsoft.com/desktop/
```

**Step 3** — Open the .pbix file

```
File → Open → select Live_project.pbix
```

**Step 4** — Refresh data if needed

```
Home → Refresh
```

**Step 5** — Explore the dashboard

```
Use slicers to filter by Region, Category, and Date Range
Click any chart to cross-filter all other visuals automatically
```

---

## 📌 How to Push to GitHub

**Step 1** — Open terminal in your project folder and initialize git

```bash
git init
```

**Step 2** — Add all project files

```bash
git add .
```

**Step 3** — Commit with a message

```bash
git commit -m "Add Superstore Power BI Dashboard"
```

**Step 4** — Connect to your GitHub repository

```bash
git remote add origin https://github.com/Meghana-b-u/superstore-powerbi-dashboard.git
```

**Step 5** — Push to GitHub

```bash
git push -u origin main
```

---

## 👤 Author

**Meghana Balappa Uppar**
- GitHub: (https://github.com/Meghana-b-u)
- LinkedIn: (https://www.linkedin.com/in/meghana-uppar-374603267/)

---

## 📄 License

This project is open source under the [MIT License](LICENSE).

---

⭐ Star this repo if you found it helpful!
