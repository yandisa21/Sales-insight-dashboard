ETL Pipeline Walkthrough
📥 Extract
Load Sales_Insights_Dashboard_project.csv using pandas (read_csv) or R’s read.csv.

Inspect schema and row count.

🧼 Transform
Missing Values:

Identify nulls in critical fields (Unit Price, Region).

Impute, drop, or flag as appropriate.

Duplicates:

Detect and remove duplicate transaction rows.

Data Types:

Convert date fields to datetime objects.

Ensure numeric fields (Unit Price, Quantity) are in correct type.

Enhancements:

Compute Total Revenue = Unit Price × Quantity.

Extract Month-Year for trend analysis.

Data Dictionary:

Provide a table of column names, types, and descriptions in Notebook 01.

💿 Load
Save the cleaned dataset as cleaned_sales_data.csv in the data/ folder for analysis notebooks.
Analysis & Visualization
Groupings & Metrics
Regional Performance: Aggregate revenue and rank regions.

Product Sales: Identify top-selling items by revenue/quantity.

Sales Rep Analytics: Calculate average sale per representative.

Monthly Trends: Visualize sales across selected months.

Visualizations (in Notebook 03)
Sales Trend Over Time — Line chart

Revenue by Product — Bar chart

Sales by Region — Pie chart

Unit Price Distribution — Boxplot

Insights & Storytelling
Include an executive summary discussing:

High-performing regions/products

Any seasonal or monthly trend

Outliers in pricing

Recommendations (e.g., focus on X product in Y region)

How to Run This Project
Clone the repo


git clone https://github.com/your-org/sales-insights-dashboard.git
cd sales-insights-dashboard
Install dependencies


pip install -r requirements.txt
Run Notebooks

Launch Jupyter
jupyter notebook
Execute notebooks in sequence:

_data_cleaning.ipynb

_data_transformation.ipynb

_analysis_and_visualization.ipynb

View Outputs

Cleaned CSV in data/


Contributions: ETL stages, analysis, visualizations, report writing, presentation design.

 License
This project is for academic purposes.
Licensed under CC BY-SA 4.0.Acknowledgements
Thanks to the module instructor and fellow classmates for guidance.

