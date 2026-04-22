# Consumer Complaints Analysis Case Study

## Project Overview
This Excel-based case study focuses on cleaning, merging, and analyzing consumer complaint data. The goal is to provide actionable insights into company performance, resolution times, and monthly trends to help stakeholders prioritize issues.

##Structure & Tasks

### Task 1: Data Integration & Preparation
* **JSON Parsing:** Converted state-to-code mapping from JSON format into a structured Excel table.
* **Data Merging:** Integrated `State_Name` into the primary `Consumer_Complaints` dataset.
* **Audit Report:** Created `Report_Task1` to analyze #N/A records, identifying missing state codes or mapping inconsistencies.

 Task 2: Date Standardization & Feature Engineering
* **Data Cleaning:** Converted inconsistent date strings into proper Excel Date objects.
* **Resolution Metrics:** Calculated `Resolution Time` (Difference between 'Date Received' and 'Date Closed').
* **Time Dimensions:** Extracted `YEAR` and `QTR (US FY)` (Q1: Jan-Mar) for time-series reporting.

Task 3: Company-Level Performance (`Report_Task3`)
Summarized data at the company level to identify:
* Total complaints per company (sorted descending).
* Timely response rates (Count and %age).
* Dispute rates and average delay in closure.

Task 4: Trend Analysis (`Report_Task4`)
* **Top 5 Analysis:** Identified the top 5 companies and top 5 most frequent complaint issues.
* **Visual Trends:** Developed Line/Area charts to visualize the monthly volume of complaints.

Task 5: Executive Dashboard (`Report_Task5`)
A high-level view providing:
* **KPIs:** YoY change in total complaints, timely responses, and average resolution time.
* **Distribution:** Breakdown of complaints by Product and Channel (Web, Phone, etc.).
* **Prioritization:** A graphical "Priority Matrix" to highlight which complaints require immediate attention based on volume and resolution lag.

## Formulas & Tools Used
* **Data Tools:** Power Query (for JSON), Text-to-Columns, Date formatting.
* **Lookup Functions:** `VLOOKUP`, `IFERROR`, `MATCH`.
* **Logic & Stats:** `AVERAGEIF`, `COUNTIFS`, `% Change` formulas.
* **Visualization:** Pivot Tables, Pivot Charts, Slicers, and Area/Line Graphs.

## Key Inferences
* **Mapping Gaps:** Significant #N/A values often result from non-standard state abbreviations in the raw data.
* **Resolution Trends:** YoY metrics indicate whether the company's customer service capacity is scaling with the volume of complaints.
* **Priority Areas:** Specific products consistently drive higher dispute rates, suggesting a need for product-level quality intervention.
