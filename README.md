# 📊 Data Analytics Power BI Assignment



---

# 📌 Project Overview

This project is a complete Power BI Data Analytics assignment covering the complete data analytics workflow.

The project includes:

- Power BI Introduction and Data Import
- Data Cleaning and Preparation
- Data Modeling and Relationships
- DAX Calculated Columns and Measures
- Power BI Visualizations
- Interactive Dashboard and Filters
- Business Insights and Recommendations

### Power BI Workflow


Data Source
     ↓
Data Import
     ↓
Data Cleaning
     ↓
Data Modeling
     ↓
Data Analysis
     ↓
Visualization
     ↓
Dashboard / Report


# 📘 Task 1: Power BI Introduction & Data Import

## 🎯 Objective

The objective of this task is to explore the Power BI interface, import a suitable dataset, view the imported data, identify available tables and columns, check column data types, and understand the basic purpose of Power BI in Data Analytics.

---

# 📊 Introduction to Power BI

Power BI is a **Business Intelligence (BI) and Data Visualization tool** developed by Microsoft.

It is used to:

- Import data from different sources.
- Clean and transform data.
- Analyze data.
- Create relationships between tables.
- Perform calculations.
- Create charts and visualizations.
- Build interactive dashboards and reports.
- Generate meaningful business insights.

---

# 🎯 Basic Purpose of Power BI in Data Analytics

The main purpose of Power BI is to transform raw data into meaningful insights through interactive reports and visualizations.

Power BI helps users:

- Understand business performance.
- Identify trends and patterns.
- Compare different categories.
- Monitor important KPIs.
- Make data-driven decisions.

---

# 🖥️ Exploring the Power BI Interface

Power BI Desktop contains several important views and sections.

## 1. Report View

Report View is mainly used to create interactive reports and dashboards.

It allows users to create:

- Charts
- Graphs
- Tables
- Cards
- KPI Visuals
- Slicers
- Interactive Reports

---

## 2. Data View

Data View is used to view the imported dataset.

It helps users:

- View rows and columns.
- Check data values.
- Understand the dataset structure.
- Identify available fields.

---

## 3. Model View

Model View is used to create and manage relationships between multiple tables.

It helps users:

- View all available tables.
- Identify common columns.
- Create relationships.
- Build a data model.

---

## 4. Power Query Editor

Power Query Editor is used for data cleaning and transformation.

It can be used to:

- Remove duplicates.
- Handle missing values.
- Change data types.
- Rename columns.
- Remove unnecessary columns.
- Replace values.
- Split columns.

---

# 📥 Dataset Import

For this project, the dataset was imported into Power BI for analysis.

The dataset can be imported from sources such as:

- Microsoft Excel
- CSV Files
- SQL Database
- Web
- SharePoint
- Other Data Sources

---

# 🔽 Steps to Import Data into Power BI

1. Open **Power BI Desktop**.
2. Click on **Get Data**.
3. Select the required data source.
4. For an Excel dataset, select **Excel Workbook**.
5. Browse and select the dataset file.
6. Select the required worksheet or table.
7. Click **Load**.


# 📘 Task 2: Data Cleaning & Preparation

Data cleaning is the process of identifying and correcting problems in raw data before analysis.
In Power BI, data cleaning is mainly performed using Power Query Editor.
## What is Power Query Editor ?

Power Query is a data transformation and ETL tool in Power BI.
It is used to:
- Remove duplicates 
- Handle missing values 
- Change data types 
- Merge tables 
- Append tables 
- Split columns 
- Pivot and unpivot data 
Power Query uses the M language behind the scenes.

## What is ETL ?
ETL = Extract, Transform, Load
•	Extract: Get data from different sources. 
•	Transform: Clean and modify the data. 
•	Load: Load the prepared data into the data model. 
## Example:
Extract data from Excel → Transform it in Power Query → Load it into Power BI

## 1. Open Power Query Editor
1.	In Power BI Desktop, click Transform Data. 
2.	Power Query Editor will open. 
3.	Perform all necessary cleaning and transformation steps.

## 2. Check for Missing or Null Values
Identify columns containing:
- Null values
- Blank values 
- Missing records 
Actions
Depending on the column:
- Remove rows with important missing values. 
- Replace null values with appropriate values. 
- Fill missing categorical values where appropriate. 
For example:
- Missing Sales → investigate or remove if invalid. 
- Missing Customer Name → replace only if a valid business rule exists. 
- Missing numerical values → replace with 0 only when logically appropriate.

## 3. Remove Duplicate Records
Duplicate records can produce incorrect results during analysis.
Steps
1.	Select the required columns or entire table. 
2.	Go to Home. 
3.	Click Remove Rows. 
4.	Select Remove Duplicates. 
This ensures that repeated records are removed

## 4. Correct Data Types
Check every column and assign the appropriate data type.
Examples:
- Dates → Date
- Quantity → Whole Number 
- Sales → Decimal Number 
- Profit → Decimal Number 
- Names and Categories → Text 
This is important for accurate calculations and analysis.

## 5. Rename Columns
Rename unclear or poorly formatted column names.
For example:
- Cust_Name → Customer Name 
- Ord_Date → Order Date 
- Sales_Amt → Sales Amount 
Clear column names improve report readability.

## 6. Remove Unnecessary Columns
Columns that are not required for analysis should be removed.
Steps
1.	Select unnecessary columns. 
2.	Right-click. 
3.	Select Remove Columns. 
This makes the dataset easier to manage and can improve performance.

## 7. Handle Text Formatting Issues
Clean text columns by:
- Removing extra spaces. 
- Correcting capitalization. 
-	Replacing incorrect values. 
-	Standardizing category names. 
Example
Before cleaning:
-	Furniture 
-	furniture 
-	FURNITURE 
After cleaning:
-	Furniture 
Power Query options:
Transform → Format → Trim
and
Transform → Format → Clean

## 8. Check for Errors
Power Query can identify data errors.
You should:
1.	Check each important column. 
2.	Identify error values. 
3.	Correct or remove invalid records. 
This improves data quality before visualization.
# Task 3: Data Modeling & Relationships

## Objective
The objective of this task is to create relationships between multiple tables using common columns and build a proper data model in Power BI.

## What is Data Modeling in Power BI?
Data Modeling is the process of organizing data from different tables and connecting those tables in a meaningful way so that Power BI can analyze the data correctly.
In simple words:
Data Modeling = Organizing tables + Creating relationships between them.

## What is a Relationship?
A relationship is a connection between two tables using a common column.

# Types of Relationships in Power BI
1. One-to-One (1:1)
One record in Table A is connected to only one record in Table B.

2. One-to-Many (1:*)
One record in one table is connected to multiple records in another table.

3. Many-to-One (*:1)
This is the same relationship viewed from the opposite direction.

4. Many-to-Many (:)
Multiple records in both tables can match multiple records in the other table.

# How to Create the Relationship in Power BI
## Method 1: Model View
1.	Click Model View from the left panel. 
2.	Identify the common column between two tables. 
3.	Drag the common column from one table to the corresponding column in another table. 
4.	Power BI opens the relationship window. 
5.	Select the correct cardinality: 
Many to One (*:1)
6.	Select the appropriate cross-filter direction. 
7.	Click OK. 


## Method 2: Manage Relationships
1.	Go to the Modeling tab. 
2.	Click Manage Relationships. 
3.	Click New Relationship. 
4.	Select the first table and column. 
5.	Select the related table and common column. 
6.	Choose: 
Cardinality: Many to One (*:1)
7.	Set the relationship as Active. 
8.	Click Save/OK.

# Explanation of the Created Data Model .
I have use Medical Table .
The data model follows a structure where:
## Fact Tables
These tables contain transactional or repeated records:
-	Diagnostics_Fact 
-	Pharmacy_Fact 
-	Visits_Fact 
## Dimension/Master Tables
These contain unique descriptive information:
-	Patient_Registry 
-	Medical_Staff 
-	Department_Master 
The fact tables are connected to the dimension tables using common keys such as:
-	Patient Code 
-	Staff Code 
-	Department Code/Name 
This structure helps Power BI perform accurate:
-	Filtering 
-	Aggregation 
-	DAX calculations 
-	Data analysis 
-	Interactive reporting 

# 1. Identify Common Columns Between Tables
The following common columns are used to connect the tables:
 
|Fact Table	      |Common Column	      |Related Table	    |Common Column
|---|---|---|---|
|Diagnostics_Fact	|Patient Ref	        |Patient_Registry	|Patient_Code
|Medical_Staff	    |Department_Name 	  |Department_Master	|Department column
|Pharmacy_Fact	   |Patient_Ref	        |Patient_Registry	|Patient_Code
|Pharmacy_Fact	    |Prescribed_By	     |Medical_Staff	    |Staff_Code
|Visits_Fact	      |Consultant_Code	    |Medical_Staff	    |Staff_Code
|Visits_Fact	      |Registered_Patient	|Patient_Registry	|Patient_Code

# 2. Relationships Created
My current data model contains the following relationships:
## Relationship 1: 
Diagnostics Fact → Patient Registry
```text
Diagnostics_Fact[Patient_Reference]
             Many (*)
                 ↓
             One (1)
Patient_Registry[Patient_Code]
```
Purpose:
One patient can have multiple diagnostic records, but each diagnostic record belongs to one patient.

Relationship Type: Many-to-One (*:1)

## Relationship 2: 
Medical Staff → Department Master
```text
Medical_Staff[Department_Name]
             Many (*)
                 ↓
             One (1)
Department_Master[Department]
```
## Purpose:
One department can have multiple medical staff members, but each staff member belongs to one department.
Relationship Type: Many-to-One (*:1)


## Relationship 3: 
Pharmacy Fact → Patient Registry
```text
Pharmacy_Fact[Patient_Ref]
          Many (*)
              ↓
          One (1)
Patient_Registry[Patient_Code]
```
## Purpose:
A patient may receive multiple prescriptions or pharmacy transactions.
Relationship Type: Many-to-One (*:1)

## Relationship 4: 
Pharmacy Fact → Medical Staff
```text
Pharmacy_Fact[Prescribed_By]
          Many (*)
              ↓
          One (1)
Medical_Staff[Staff_Code]
```
## Purpose:
One doctor or medical staff member can prescribe medicines to multiple patients.
Relationship Type: Many-to-One (*:1)

## Relationship 5: 
Visits Fact → Medical Staff
```text
Visits_Fact[Consultant_Code]
        Many (*)
            ↓
        One (1)
Medical_Staff[Staff_Code]
```
## Purpose:
One medical staff member or consultant can attend multiple patient visits.
Relationship Type: Many-to-One (*:1)

## Relationship 6: 
Visits Fact → Patient Registry
```text
Visits_Fact[Registered_Patient]
          Many (*)
              ↓
          One (1)
Patient_Registry[Patient_Code]
```
## Purpose:
One patient can visit the hospital multiple times, creating multiple records in the Visits Fact table.
Relationship Type: Many-to-One (*:1)
## Before doing Data Modeling the Model view showing:
![Before Data Modeling](Before%20Data%20Modeling.png)
## After doing Data Modeling the Model view showing :
![After Data Modeling](After%20Data%20Modeling.png)

# Task 4: DAX Calculated Columns & Measures

### What is DAX?
DAX (Data Analysis Expressions) is a formula language used in Power BI to create:
-	Calculated Columns 
-	Measures 
-	Calculated Tables

## 1. Difference Between Calculated Column and Measure
Calculated Column
A calculated column performs a calculation for each row of a table.

Measure
A measure performs calculations dynamically based on filters and visuals.
The result changes when you use:
•	Slicers 
•	Filters 
•	Charts 

## 2. DAX Measures :
### Measure 1: Total Amount / Total Sales
             Total Sales = SUM(Orders[Sales])

### Measure 2: Average Sales Amount
         Average Sales Amount = AVERAGE(Orders[Sales])

### Measure 3: Total Number of Records
         Total Orders = COUNTA(Orders[Order ID])

### Measure 4: Max Sales Value 
       Max Sales = MAX(Orders[Sales])

### Measure 5: Min Sales Value 
        Min Sales Value = MIN(Orders[Sales])

### Measure 6: Total Revenue 
         Total Revenue = sum(Orders[Total Revenue])

### Measure 7 : Total Profit 
           Total Profit = SUM(Orders[Profit])


### Measure 8 : Profit % 
      Profit % = DIVIDE( [Total Profit], [Total Revenue Amount] , 0)

## 3. How to Create a Measure in Power BI
1.	Go to the Data View or Report View. 
2.	Select the table where you want to create the measure. 
3.	Right-click the table. 
4.	Select New Measure. 
5.	Enter the DAX formula.
6.	Press ENTER

## 4. Display the Results
To display the results:
1.	Go to Report View. 
2.	Select the Card visual. 
3.	Drag the measure into the card.
## Output :
![Measured Cards](Measured%20Cards.png)

# Task 5: Power BI Visualizations
## Objective
The objective of this task is to create different Power BI visualizations to represent the data clearly and identify trends, comparisons, patterns, and business insights.

## What is Data Visualization?
Data Visualization is the graphical representation of data using charts, graphs, tables, and other visual elements.
Power BI visualizations help convert raw data into meaningful and easy-to-understand information.

### Visualizations to Create
Based on My Financials dataset, I Have create the following visualizations.

## 1. Line Chart – Total Sales by Month
### Visual:
Line Chart
### Fields:
-	X-Axis: Month Name 
-	Y-Axis: Sales 
### Title:
Total Sales by Month
### Purpose:
This visualization shows the monthly sales trend and helps identify months with high and low sales.

## 2. Clustered Column Chart – Total Sales by Segment and Year
### Visual:
Clustered Column Chart
### Fields:
-	X-Axis: Segment 
-	Y-Axis: Sales 
-	Legend: Year 
### Title:
Total Sales by Segment and Year
### Purpose:
This chart compares sales performance across different business segments and years.
## 3. Donut Chart – Profit by Product
### Visual:
Donut Chart
### Fields:
-	Legend: Product 
-	Values: Profit 
### Title:
Profit by Product
### Purpose:
This visualization shows the contribution of each product to total profit.

## 4. Line and Clustered Column Chart – Sales and Profit by Country
### Visual:
Line and Clustered Column Chart
### Fields:
-	X-Axis: Country 
-	Column Y-Axis: Sales 
-	Line Y-Axis: Profit 
### Title:
Sales and Profit by Country
### Purpose:
This visualization compares sales and profit across different countries.

## 5. Table Visual – Product, Segment and Gross Sales
### Visual:
Table
### Fields:
-	Product 
-	Segment 
-	Gross Sales 
### Title:
Product-wise Gross Sales Details
### Purpose:
This visual provides detailed information about product sales and segments.

## 6. KPI Cards
### 1. Total Sales
1.	Select the Card visual. 
2.	Drag the Sales column into the card. 
3.	Power BI will automatically calculate the Sum of Sales. 
Set the title as:
Total Sales

### 2. Total Profit
1.	Add a Card
2.	Drag the Profit column. 
3.	Set aggregation to Sum. 
Result:
Sum of Profit
Title:
Total Profit

### 3. Total Gross Sales
1.	Add a Card. 
2.	Drag Gross Sales into the card. 
3.	Select aggregation as Sum. 
Title:
Total Gross Sales

### 4. Total Units Sold
1.	Add a Card. 
2.	Drag Units Sold into the card. 
3.	Select aggregation as Sum. 
Title:
Total Units Sold

### 5. Profit %
Profit % = DIVIDE( [Total Profit], [Total Sales], 0 )
- After creating the measure:
Measure Tools → Format → Percentage
1.	Add a Card. 
2.	Drag Measured Profit % into the card.
## Final dashboard :
![Financial Sales Dashboard](Financial%20Sales%20Dashboard.png)

# Task 6: Interactive Dashboard & Filters


## Objective :
To design and develop an interactive Power BI dashboard using KPI cards, multiple visualizations, slicers, and filters to enable users to explore data, analyze business performance, identify trends, and gain meaningful insights for decision-making.

## What is Visualization?
Visualization is the graphical representation of data using charts, graphs, maps, tables, and other visual elements.
In Power BI, visualizations help convert raw data into easy-to-understand information and insights.

Different Types of Visualizations in Power BI
### 1. Bar Chart
Used to compare values between different categories.
Best for:
-	Comparing categories 
-	Ranking products 
-	Comparing regions

### 2. Column Chart
Similar to a bar chart, but displayed vertically.
Best for:
-	Comparing sales 
-	Comparing profit 
-	Category-wise analysis

### 3. Line Chart
Used to show trends over time.
Best for:
-	Monthly trends 
-	Yearly trends 
-	Revenue growth 

### 4. Pie Chart
Shows how each category contributes to the total.
Best for:
-	Percentage contribution 
-	Small number of categories


### 5. Donut Chart
Similar to a Pie Chart but has a hole in the center.
Best for:
-	Contribution analysis 
-	Product-wise profit 
-	Category distribution

### 6. Area Chart
Shows trends and emphasizes the magnitude of values over time.
Best for:
-	Sales trends 
-	Revenue trends 
-	Growth over time

### 7. Clustered Column Chart
Compares multiple values across categories.
Best for:
-	Comparing multiple measures 
-	Year-wise comparison 
-	Category comparison

### 8. Stacked Column Chart
Shows the total and the contribution of different categories.
Best for:
-	Contribution to total 
-	Category comparison

### 9. Combo Chart
Combines two charts, usually:
-	Column Chart 
-	Line Chart
Best for:
-	Comparing two different measures 
-	Comparing Sales vs Profit

### 10. Scatter Chart
Shows the relationship between two numerical variables.
Best for:
-	Correlation analysis 
-	Finding outliers 
-	Relationship analysis
### 11. Treemap
Displays data using rectangles of different sizes.
Best for:
-	Hierarchical data 
-	Category contribution 
-	Comparing proportions

### 12. Map
Displays geographical data.
Best for:
-	Country-wise analysis 
-	State-wise sales 
-	Regional performance

### 13. Table
Displays detailed data in rows and columns.
Best for:
-	Detailed information 
-	Record-level analysis

### 14. Matrix
Similar to a Pivot Table in Excel.
Best for:
-	Hierarchical analysis 
-	Summary reports 
-	Comparing multiple dimensions

### 15. Card
Displays a single important KPI.
Best for:
-	KPIs 
-	Important summary values

### 16. Slicer
A slicer is an interactive filtering visualization.
When a user selects a value, all connected visuals can update.

I have create a interactive AMAZON PRIME SALES DASHBOARD.

### Dashboard Title
SALES ANALYSIS | AMAZON PRIME

## 1. KPI Cards
The dashboard contains 3 KPI Cards.
### 1. Total Sales 
        Total Sales = sum('Amazon Prime Data'[Price(Dollar)])
- After creating the measure:
1.	Add a Card. 
2.	Drag Measured Total Sales into the card. 
### 2. Total Product Description 
         Total Product Description = DISTINCTCOUNT('Amazon Prime Data'[Product Description ])
- After creating the measure:
1.	Add a Card. 
2.	Drag Measured Total Product Description into the card. 
### 3. Total No of Reviews 
                 Total No of Reviews = SUM('Amazon Prime Data'[Number of reviews])
- After creating the measure:
1.	Add a Card. 
2.	Drag Measured Total no of reviews into the card. 
These KPI cards provide a quick summary of the overall dataset.

## 2. Slicers / Filters
The dashboard contains 3 interactive slicers on the left side.
### Quality Filter
Users can filter the dashboard based on quality, such as:
-	Prime Video 
-	Blu-ray 
-	DVD 
-	4K 
-	Multi-Format 
### Director Filter
Users can select a specific Director to analyze movies and sales associated with that director.
### Movie Type Filter
Users can filter the data based on different Movie Types.
These filters allow all connected visuals and KPI cards to update dynamically.

## 3. Visualizations Used
The dashboard contains more than the required 4 visualizations.
## Visualization 1: Line Chart
### Title:
Total Movie Count by Release Year (2010–2023)
This chart displays the number of movies released each year.
### Purpose:
-	Identify movie release trends. 
-	Find years with the highest number of movies. 
-	Compare movie counts over time.

## Visualization 2: Bar Chart
### Title:
Total Sales by Movie Type
This visualization compares total sales across different movie types.
### Purpose:
-	Identify the highest-selling movie type. 
-	Compare sales performance between movie classifications.

## Visualization 3: Donut Chart
### Title:
Total Sales by Quality
This chart shows how total sales are distributed among different movie quality formats.
### Purpose:
-	Analyze the contribution of each quality type. 
-	Identify the quality category generating the highest sales.

## Visualization 4: Bar Chart
### Title:
Top 5 Movies by Total Sales
This visualization displays the five movies generating the highest sales.
### Purpose:
-	Identify the best-selling movies. 
-	Compare the sales performance of the top movies. 

## Visualization 5: Bar Chart
### Title:
Top 5 Movies by Reviews
This chart displays the five movies with the highest number of reviews.
### Purpose:
-	Identify the most reviewed movies. 
-	Analyze audience engagement and popularity.
## Final dashboard image 
![Amazon Prime Sales Dashboard](Amazon%20Prime%20Sales%20Dashboard.png)

# Task 7: Business Insights & Recommendations

## Objective :
The objective of this task is to analyze the Power BI dashboard, identify meaningful business insights, recognize important trends and patterns, and provide data-driven recommendations.
## Insights
Business Insights from the Amazon Prime Dashboard .

### Insight 1: Movie Count Increased Significantly Over Time
The Total Movie Count by Release Year chart shows an overall increasing trend in movie releases.

### Insight 2: CC Movie Type Generates the Highest Sales
According to the Total Sales by Movie Type chart:
-	CC generated the highest sales of approximately $30K. 
-	R generated approximately $21K. 
-	PG-13 generated approximately $13K. 
-	TV-PG generated the lowest sales of approximately $2K. 
Highest Performing Movie Type
🥇 CC – approximately $30K
Lowest Performing Movie Type
📉 TV-PG – approximately $2K

### Insight 3: Prime Video Quality Dominates Total Sales
The Total Sales by Quality chart shows that:
-	Prime Video generated approximately $68.13K, representing 78.72% of total sales. 
-	Other quality formats such as Blu-ray and DVD contribute significantly less.

## Business Recommendations
### Recommendation 1: Focus More on High-Performing Movie Types
The CC movie type generates approximately $30K, making it the highest-performing category.
### Recommendation
Amazon Prime should analyze the characteristics of successful CC movies and consider acquiring, promoting, or producing more content with similar characteristics.

### Recommendation 2: Continue Investing in Prime Video Content
Prime Video quality contributes approximately:
$68.13K or 78.72% of total sales
### Recommendation
The business should continue investing in Prime Video content because it is the dominant source of sales and has the strongest customer preference.
Recommendation 3: Promote Highly Reviewed Movies
God's Country has:
-	$8.4K in sales 
-	508K reviews 
### Recommendation
Movies receiving high customer engagement and reviews should receive additional promotion because they have the potential to generate higher sales.


