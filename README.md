🚀 Project Roadmap: FinSight360 (Excel → Power BI)
🔹 Phase 1: Data Preparation in Excel

Components used:

Raw dataset (Date, Sales, Target_Sales, Forecast_Sales).

Excel Power Query.

Excel VBA Macros.

Actions you took:

Imported dataset into Excel.

Used Power Query to clean data:

Selected only required columns (Date, Sales, Target, Forecast).

Added Index Column and then transformed it into a Date column.

Created a structured table.

Added a Month column (via formula and later automated in VBA).

Built formulas:

Forecast functions (Forecast.LINEAR).

Profit/Loss comparison (Actual vs Target).

Created VBA Macros + Buttons:

Button 1: Refresh Forecast (auto-refresh all queries & calculations).

Button 2: Check Profit/Loss → shows popup + colors row based on result.

Button 3: Update Dashboard → auto-updates totals and accuracy % in dashboard.

Button 4: Clear Profit/Loss → resets Profit/Loss column.

Built an Excel Dashboard:

Line chart: Actual vs Target vs Forecast.

Conditional formatting (Profit = Green, Loss = Red).

KPI cards (Total Sales, Target, Accuracy %).

Slicer (Date/Month filter).

✅ Excel outcome: You had a semi-automated dashboard showing actual vs target, forecasting, and Profit/Loss status — with macros for live interactivity.

🔹 Phase 2: Migration to Power BI

Components used:

Power BI Desktop.

Excel file (FinSight360_Forecast.xlsx).

Power BI visuals (Cards, Line Chart, Column Chart, Slicer).

DAX Measures.

Actions you took:

Imported Excel data into Power BI (Get Data → Excel → Load table).

Built DAX measures to replace Excel formulas/macros:

Total Sales = SUM(Sales).

Total Target Sales = SUM(Target_Sales).

Total Forecast Sales = SUM(Forecast_Sales).

Profit Days = COUNTROWS where Sales > Target.

Loss Days = COUNTROWS where Sales < Target.

Equal Days = COUNTROWS where Sales = Target.

Accuracy % = % of days Actual ≈ Target (±5% tolerance).

Variance = Sales – Target.

%Variance = Variance ÷ Target.

Designed Power BI visuals:

Line chart → Date on X-axis, Actual vs Target vs Forecast lines.

Card visuals → Profit Days, Loss Days, Accuracy %, Total Sales, Total Target.

Bar chart → Profit vs Loss by Month.

Slicer → Month filter for interactive drilldown.

Applied formatting:

Green for Profit, Red for Loss.

KPI color logic (Accuracy % traffic light: Green >90%, Yellow 70–90%, Red <70%).

✅ Power BI outcome: A fully interactive, professional BI dashboard with KPIs, trend lines, and slicers — easy for recruiters/managers to explore.

🔹 Phase 3: Insights & Storytelling

Key actions for presentation:

Highlight automation in Excel (macros + forecasting).

Show how you migrated to Power BI for modern visualization.

Demonstrate insights:

“In X% of days, Actual Sales matched or exceeded Target.”

“Forecast accuracy is ~85%, showing reliability of predictions.”

“Profit/Loss distribution by month reveals seasonal patterns.”