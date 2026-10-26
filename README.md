# BANK-LOAN-REPORT-EXCEL
Bank Loan Report Dashboard | Excel
An interactive Microsoft Excel dashboard designed to monitor loan
portfolio performance, compare loan status groups, and highlight areas
that may require further credit-risk investigation.
Project Overview
This project uses Excel to turn loan data into a visual dashboard for
management-level portfolio monitoring. It summarizes loan applications,
funded amounts, amounts received, interest rates, and borrowers'
debt-to-income ratios (DTI).
The dashboard includes KPI cards, loan-status comparisons, monthly
trends, and filters for exploring results by loan grade and loan
purpose.
Project Objectives
•	Monitor total loan applications, funded amounts, and amounts
received.
•	Compare Good Loan and Bad Loan application shares.
•	Review loan status and identify potential risk areas.
•	Track average interest rate and average DTI.
•	Display Month-to-Date (MTD) metrics and Month-over-Month (MoM)
movement.
•	Provide a concise, interactive view of portfolio performance.
Key Performance Indicators
KPI Reported Values -
Total Loan Applications 38.6K
Total Funded Amount $435.8M
Total Amount Received $473.1M
Average Interest Rate Approximately 12.05%
Average Debt-to-Income Ratio (DTI) 13.33%
Values are based on the dashboard summary. Exact displayed values may
vary with rounding and filters.
MTD and MoM
•	MTD (Month-to-Date): Measures performance from the beginning of
the current month through the latest available date.
•	MoM (Month-over-Month): Measures the percentage change compared
with the previous month.
A common MoM calculation is:
=(Current_Month-Previous_Month)/Previous_Month
Format the result as a percentage. Handle blank or zero previous month
values to avoid division errors.
Dashboard Features
•	Executive KPI cards: Applications, funded amount, amount
received, average interest rate, and average DTI.
•	Good Loan vs. Bad Loan comparison: Shows the share of
applications in each group.
•	Loan status analysis: Compares Fully Paid, Current, and Charged
Off records.
•	Funding and receipt analysis: Compares funded amounts with
amounts received.
•	Loan purpose analysis: Supports comparison across different
borrowing purposes.
•	Monthly trend: Displays movement over time.
•	Interactive filters: Explore the dashboard by loan grade (A--G)
and loan purpose.
Data Description
The dashboard summarizes loan records using these dimensions and
measures.
Dimensions -
•	Loan status: Fully Paid, Current, Charged Off
•	Loan grade: A to G
•	Loan purpose: Examples include car, credit card, debt
consolidation, education, home improvement, and house
Measures
•	Number of loan applications
•	Funded amount
•	Amount received
•	Average interest rate
•	Average debt-to-income ratio (DTI)
•	MTD and MoM indicators
Data Cleaning and Transformation
The project workflow includes the following checks and transformations:
1.	Standardize loan status, grade, and purpose labels.
2.	Check loan IDs for duplicate records.
3.	Review missing or null values and document how they are handled.
4.	Create a loan-status grouping for Good Loans and Bad Loans.
5.	Calculate or summarize average interest rate and DTI.
6.	Prepare MTD and MoM measures for trend monitoring.

Example Excel formula for the loan-status group, assuming the source is
an Excel Table:
=IF(OR([@[loan_status]]="Fully Paid",[@[loan_status]]="Current"),
"Good Loan",
IF([@[loan_status]]="Charged Off","Bad Loan",""))
This classification follows the project's stated grouping. Confirm that
it matches the definitions required by the source dataset or business
rules.
Key Insights
1.	Good Loans account for approximately 86.18% of loan
applications.
2.	The portfolio contains 38,576 loan applications.
3.	Total funded amount is $435.8M, while total amount received is
$473.1M.
4.	Charged-off loans account for $65.5M in funded amount and
$37.3M in amount received. The $28.2M difference should be
investigated; it should not automatically be treated as a loss or
outstanding principal without validating the dataset's definitions.
5.	The dashboard reports an overall average interest rate of
approximately 12.05% and an average DTI of 13.33%.
Validation note: Claims comparing interest rate or DTI across
individual loan status should be included only after confirming the
status-level calculations in the source workbook.
Tools and Skills
•	Microsoft Excel
•	Data cleaning and transformation
•	KPI reporting
•	PivotTables and charts
•	Dashboard design and data visualization
•	Loan portfolio and repayment-status analysis
•	Trend analysis using MTD and MoM metrics
Intended Users
•	Banking and lending management
•	Credit and risk teams
•	Finance teams
•	Business and operations teams
•	Senior leadership
The dashboard is intended as a portfolio-monitoring aid. It does not
replace a formal credit-risk assessment or a complete economic analysis.
How to Use
1.	Download or clone this repository.
2.	Open the Excel workbook (PROJECT.xlsx) in Microsoft Excel.
3.	Navigate between the Summary and Details views, where
available.
4.	Use the loan-grade and loan-purpose filters to explore the data.
5.	Review KPI cards and charts together, and verify filtered values
before drawing conclusions.
Limitations and Notes
•	KPI values may be rounded in the dashboard.
•	Findings depend on the completeness, quality, and definitions of the
source dataset.
•	The difference between funded amount and amount received is not
necessarily equivalent to a financial loss.
•	If the workbook uses PivotTables, refresh them after updating the
source data.
•	Confirm formulas, filter behavior, and all reported insights before
using the dashboard for business decisions.
Conclusion
This project demonstrates the use of Excel for interactive reporting and
exploratory loan portfolio analysis. It brings important metrics into
one view, helps compare loan-status groups, and highlights questions
that may require further investigation.
________________________________________
Project type: Data Analytics Portfolio Project
Tool: Microsoft Excel
Focus: Loan Portfolio Analysis and Dashboard Reporting

