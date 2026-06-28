# mannatgill_2507628_part4_tableau_dashboardPart 4: Tableau Executive Dashboard & Data Storytelling
Student Information

Name: Mannat Gill
Student ID: 2507628

Business Problem Summary

A retail leadership team requires an executive dashboard to monitor overall business performance and support strategic decision-making. The dashboard aims to provide insights into sales trends, profitability, customer segments, regional performance, shipping efficiency, discount impact, and return patterns.

The objective is to transform raw sales data into an interactive Tableau dashboard that enables leadership to quickly identify business opportunities, operational risks, and areas requiring improvement.

Dataset Description

The dataset contains transactional retail sales information used for dashboard creation. Key fields include:

Order Date
Sales
Profit
Discount
Quantity
Region
State
Category
Sub-Category
Customer Segment
Ship Mode
Delivery Days
Returns
Order ID

The dataset combines geographical, categorical, and numerical fields suitable for executive reporting.

Tableau Workbook Description

The Tableau packaged workbook (executive_dashboard.twbx) contains:

Sales Trend View
Regional Performance View
Category Profitability View
Customer Segment View
Shipping Performance View
Discount vs Profit View
Return Analysis View

The workbook also includes KPI cards, interactive filters, dashboard actions, and calculated fields to support leadership decision-making.

Calculated Fields Created

The following calculated fields were created in Tableau:

1. Profit Margin
Profit / Sales

Measures profitability for each sale.

2. Cost
Sales - Profit

Estimates the cost associated with each sale.

3. Average Order Value (AOV)
SUM(Sales) / COUNTD(Order ID)

Measures the average revenue generated per order.

4. Return Rate
SUM(Returned Orders) / COUNTD(Order ID)

Measures the proportion of returned orders.

5. Shipping Delay Bucket

Example logic:

0–2 Days → Fast
3–5 Days → Standard
6+ Days → Delayed

Used to analyze shipping performance.

Dashboard Components

The executive dashboard includes:

KPI Card – Total Sales
KPI Card – Total Profit
KPI Card – Profit Margin
Sales Trend Line Chart
Regional Performance Bar Chart
Category Profitability Chart
Customer Segment Comparison
Shipping Performance Chart
Discount vs Profit Scatter Plot
Return Analysis Chart

Each visualization answers a specific business question and contributes to the overall dashboard story.

Filters and Dashboard Interactions

The dashboard includes interactive filters for:

Region
Category
Customer Segment
Order Date
Ship Mode

Dashboard actions allow users to click one chart and automatically filter related visualizations, improving exploration and decision-making.

Key Business Insights

The dashboard highlights several important business insights, including:

Sales trends over time.
Regional differences in sales and profitability.
Most and least profitable product categories.
Customer segment performance.
Relationship between discount levels and profitability.
Shipping delays by shipping mode.
Return patterns across products and regions.
Opportunities for improving operational efficiency and revenue growth.

Detailed insights are documented in:

outputs/business_insights.md
Dashboard Story Summary

The executive dashboard tells a complete business story by connecting multiple performance indicators rather than presenting isolated charts.

The dashboard helps leadership answer questions such as:

Which regions generate the highest sales?
Which product categories generate the greatest profit?
Are higher discounts reducing profitability?
Which shipping methods experience the greatest delays?
Which customer segments present the greatest opportunities?
Where are return rates creating business risk?

The complete dashboard narrative is available in:

outputs/dashboard_story.md
Assumptions

The following assumptions were made:

Date fields were correctly recognized by Tableau.
Geographic fields were assigned appropriate geographic roles.
Sales and Profit values are stored as numerical measures.
Return information accurately reflects returned orders.
Delivery days represent the number of days between shipment and delivery.
Limitations

The dashboard has several limitations:

It reflects historical business performance only.
Future sales cannot be predicted directly from dashboard visualizations.
External factors such as economic conditions or competitor actions are not represented.
Dashboard insights depend on the quality and completeness of the source dataset.
Repository Structure
part4_tableau_dashboard/

├── data/
│   └── dashboard_sales_data.xlsx
│
├── tableau/
│   └── executive_dashboard.twbx
│
├── outputs/
│   ├── dashboard_story.md
│   ├── business_insights.md
│   └── chart_selection_justification.md
│
├── screenshots/
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   └── filter_interaction_view.png
│
└── README.md
Screenshots Included

The repository includes the following dashboard screenshots:

full_dashboard.png – Complete executive dashboard.
sales_trend_view.png – Sales trend over time.
regional_performance_view.png – Sales and profit by region.
category_profitability_view.png – Profitability by category and sub-category.
filter_interaction_view.png – Demonstration of interactive filters and dashboard actions.
Conclusion

This Tableau executive dashboard transforms retail sales data into an interactive decision-support tool for leadership. By combining calculated fields, meaningful visualizations, KPI cards, filters, and business storytelling, the dashboard enables users to identify trends, evaluate performance, monitor operational risks, and make informed strategic decisions.
