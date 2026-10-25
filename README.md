# Sales Performance Dashboard

An interactive Power BI dashboard that tracks sales performance and each salesperson's progress toward their goal. It is built with DAX measures, dynamic dimension switching and custom SVG visuals.

![Sales page](images/sales-page.png)
![Progress to Goal page](images/progress-to-goal.png)

## Business Question
How are sales performing over time, who is driving them, and which salespeople are on track to hit their goals?

## Data
- **Source:** Sample dataset provided in Christine Payton's Power BI course on Udemy
- **Tables:** Sales, Employees, Sales Goals, Date
- **Note:** This project uses course sample data only. It contains no real company information.

## Dashboard Pages

### 1. Sales
- **Current Year Sales** card for a quick headline number
- **Sales by Month** line chart and column chart for trends
- **Sales by Person** bar chart that switches dimension using a field parameter slicer
- **Day of Week vs Month** matrix showing sales counts

### 2. Progress to Goal
- Table showing each salesperson's progress toward their goal with a custom **SVG bullet chart**
- Color-coded progress: green (goal met), yellow (50% or more), red (below 50%)
- Red dot indicator for people at or below 20% of goal
- Sales trend sparklines
- **Cumulative sales** area chart

## Key Techniques
- Custom DAX measure that generates **SVG graphics** inside a table
- **Field parameters** so users can change the dimension on the bar chart
- Time intelligence measures, including current year and same period last year
- Sparklines and conditional formatting
- Whole-number rounding in the SVG measure to avoid decimal-separator problems on regional settings that use a comma

## Key Insights
- [Finding 1, e.g. "Sales peaked in (month)"]
- [Finding 2, e.g. "X of Y salespeople met their goal"]
- [Finding 3, e.g. "Several salespeople are below 50% of goal"]

## Files
- `Sales_Dashboard.pbix`: the Power BI file (open in Power BI Desktop)
- `images/`: dashboard screenshots
- `DAX-measures.md`: the DAX measures used

## Tools
Power BI Desktop, DAX, Power Query

## Credits
Dataset and project brief from Christine Payton's Udemy course. I customized the dashboard, including the SVG bullet chart and the Red Dot indicator, with my own modifications to the DAX measures.

## Author
[Payton] | [www.linkedin.com/in/payton-adams-2a1415386]
