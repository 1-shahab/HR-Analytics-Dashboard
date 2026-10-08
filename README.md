# IBM HR Analytics Dashboard

This project is a comprehensive HR Analytics Dashboard built in Microsoft Excel. It focuses on visualizing employee data to understand key drivers of attrition, job satisfaction, and employee demographics.

## 📊 Dashboard Overview
![Dashboard Preview](https://github.com/1-shahab/HR-Analytics-Dashboard/blob/main/assets/Screenshot%202026-10-05%20053405.png))

## 🎯 Key Objectives
- To identify patterns and trends in employee attrition.
- To provide actionable insights regarding job satisfaction, salary distribution, and work-life balance.
- To create a user-friendly, interactive analytical tool for stakeholders.

## 🛠 Methodology & Technical Approach
A key challenge in HR data analytics is the **"Denominator Trap,"** where filtering data leads to incorrect percentage calculations. To ensure data integrity, this project employs a robust calculation method:

1.  **Helper Column Strategy:** I implemented an `Attrition_Flag` column using the following formula:
```excel
=IF(D2="Yes", 1, 0)
```
2.  **Aggregation: Instead of standard count filters, the dashboard utilizes the Average aggregation on this helper column. This ensures that percentages remain mathematically accurate regardless of the filters applied via slicers.
3.  **Visualization: Designed with a “Canvas” approach—removing UI noise (gridlines, page breaks) to focus strictly on data storytelling.
🚀 Key Features
Interactive Filtering: Use slicers for Department, Gender, and MaritalStatus to drill down into specific employee segments.
Dynamic KPI Tracking: Real-time calculation of key metrics.
Modern UI: Clean, professional aesthetic optimized for executive presentations.
📁 Repository Structure
HR.xlsx: The main dataset and dashboard file.
assets/: Contains dashboard screenshots for visual reference.
Data_Dictionary.md: Definitions of the columns used in the dataset.
🛠 Tools Used
Microsoft Excel: Pivot Tables, Slicers, Data Visualization, and Pivot Charts.
💡 Future Improvements
Integrate with Power Query for automated data refreshing.
Implement predictive modeling (e.g., Logistic Regression) to forecast future attrition.
