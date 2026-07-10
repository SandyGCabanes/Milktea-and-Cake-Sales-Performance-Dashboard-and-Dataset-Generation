# Q2 Milktea and Cake Sales Performance Dashboard and Dataset Generation
### An end-to-end Python data pipeline and automated Excel dashboard, tracking revenue, delivery channels and product trends across 5 store locations.

## Project Overview
This project demonstrates how to solve a common retail problem: tracking down why sales dropped over a quarter. Because real store data is confidential, a custom Python script was used to build a highly realistic transaction dataset from scratch.  Seasonal shifts and branch performance drops are included to run a proper root-cause analysis.

## Project Navigation
Select the document you want to review:

* **For Business Leaders:** Read the [Q2 Performance & Actionable Insights Report](Q2_Performance_Report.md). This shows how operational bottlenecks are pinpointed and turned into clear, practical business advice.
    
* **For Technical Reviewers:** Read below to see how the data was built, the tools used, and the design choices behind the project.[Python code flowchart](config_routing_map.html.pdf)
*Note: I am happy to walk through the backend Python code and logic during an interview.*

## Challenge, Solution and Scope

### The Data Challenge
* **The Problem:** Real company data is private, but standard public datasets are usually too clean and perfect. They lack the messy, day-to-day operational variations and regional trends seen in a real business.
* **The Solution:** A custom Python script generated a realistic dataset from scratch. Seasonal trends, differences between branches, and specific sales drops were intentionally built in to mimic a live business. SQLite was used to inspect and clean up the data at every step.

### Case Study Scope
The data simulates a fast-casual retail operation with five branches selling milk tea and cakes:
* **Volume:** 6 months of continuous transaction data.
* **Product Groups:** Items are grouped into categories like "Cheesecake Slice" or "Milk Tea Classic." To make it look realistic, item prices fluctuate naturally within a normal range instead of staying completely frozen.

### What Was Left Out
To keep the focus entirely on buying patterns and sales analysis, secondary administrative details were skipped:
* No marketing promos, senior citizen discounts, or PWD tracking.
* No tax or VAT breakdowns.
* No complex payment issues like partial refunds or canceled transactions.

### Core Skills Demonstrated
1. **Dataset Generation:** Creating mock sales logs that actually look like real-world retail shopping habits.
2. **Root-Cause Analysis:** Drilling down into product categories, delivery apps/walk-ins and branches to find the exact reason for a sales dip.
3. **Data Prep:** Exploring database tables in SQLite and organizing clean data summaries for Excel.

## Data Governance & Safety
* **Public View:** Executive report and the final secure Excel file are available here in the repository. Backend flowchart for the python script is also included.
* **Private Files:** The raw Python script and backend SQLite database are kept private to protect the underlying logic, for IP reasons. (Available during interviews.)
* **Validation:** The script runs automated checks at every stage to ensure the final numbers perfectly match the planned business scenario.

## Excel Dashboard Setup
The final deliverable is a clean, easy-to-read Excel [workbook](pearltea_transactions_github.xlsx).
* **Data Security:** All raw, row-by-row transaction data was removed after aggregation to protect privacy and keep the file size light.
* **User Interface:** The dashboard uses standard formulas to pull data from a summary tab. This keeps the reporting cards fully interactive but prevents anyone from extracting raw, underlying transaction data.
