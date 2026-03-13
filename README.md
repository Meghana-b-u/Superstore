📊 Superstore Sales Analysis — Power BI Dashboard
A live interactive Sales Analytics Dashboard built in Power BI Desktop using the Superstore retail dataset. The dashboard provides insights into sales performance across regions, categories, segments, and shipping modes.

📸 Dashboard Preview
<img width="1003" height="743" alt="Screenshot 2026-03-13 225110" src="https://github.com/user-attachments/assets/253e4df6-2cfc-4cbe-a814-fdd7d504c719" />


Key highlights: Dark navy header, KPI cards, interactive slicers, and 6 chart visuals with cross-filtering enabled.


📁 Project Structure
superstore-powerbi-dashboard/
│
├── Superstore_Analysis.pbix       # Main Power BI file
├── train.csv                      # Source dataset (9,800 rows)
├── dashboard-screenshot.png       # Dashboard preview image
└── README.md                      # Project documentation

📋 Dataset
PropertyDetailsSourceKaggle — Superstore DatasetRows9,800 ordersColumns18 columnsDate Range2015 – 2018
Columns Used
ColumnDescriptionOrder IDUnique order identifierOrder DateDate the order was placedShip DateDate the order was shippedShip ModeShipping class (Standard, First, Second, Same Day)Customer NameName of the customerSegmentCustomer segment (Consumer, Corporate, Home Office)RegionUS region (West, East, Central, South)CategoryProduct category (Furniture, Technology, Office Supplies)Sub-CategoryProduct sub-category (Phones, Chairs, Storage, etc.)SalesRevenue generated per order

📊 Dashboard Visuals
VisualTypeFields UsedTotal SalesKPI CardSUM(Sales)Total OrdersKPI CardDISTINCTCOUNT(Order ID)Avg Order ValueKPI CardTotal Sales / Total OrdersSales by Sub-CategoryHorizontal Bar ChartSub-Category, SalesSales by CategoryHorizontal Bar ChartCategory, SalesSales by RegionDonut ChartRegion, SalesSales by SegmentPie ChartSegment, SalesSales by MonthLine ChartMonth, SalesTop Sub-CategoriesTableSub-Category, Sum of SalesRegion FilterTile SlicerRegionCategory FilterTile SlicerCategoryDate FilterDate Range SlicerOrder Date

🧮 DAX Measures
dax-- Total Sales
Total Sales = SUM('train'[Sales])

-- Total Orders
Total Orders = DISTINCTCOUNT('train'[Order ID])

-- Average Order Value
Avg Order Value = DIVIDE([Total Sales], [Total Orders])

🔑 Key Insights

Phones and Chairs are the top 2 sub-categories with ₹3.27M and ₹3.22M in sales respectively
West region leads with 31.4% of total sales (₹710K)
Consumer segment dominates with 50.7% of all sales
Technology is the highest performing category at ₹0.83M
Standard Class is the most used shipping mode across all orders
Total revenue across all years: ₹19,90,893


🛠️ Tools & Technologies
ToolPurposePower BI DesktopDashboard creation and visualizationPower Query EditorData transformation and cleaningDAXCustom measures and calculationsCSV (Kaggle)Source data

🚀 How to Run This Project

Clone this repository

bash   git clone https://github.com/Meghana-b-u/superstore-powerbi-dashboard.git

Open Power BI Desktop

Download free from Microsoft Power BI


Open the .pbix file

File → Open → select Superstore_Analysis.pbix


Refresh the data (if needed)

Home → Refresh


Explore the dashboard

Use slicers to filter by Region, Category, and Date Range
Click any chart to cross-filter all other visuals

👤 Author
Meghana Balappa Uppar

GitHub: @meghana-b-u
LinkedIn: meghana-uppar-374603267


📄 License
This project is open source and available under the MIT License.

⭐ If you found this project helpful, please give it a star on GitHub!
