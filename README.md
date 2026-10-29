# Credit Card Financial Report

> Guided practice project (Nov 2024), built by following Rishabh Mishra's YouTube tutorial. The dataset and the report design come from the tutorial; I rebuilt it step by step.

A weekly credit card report in Power BI, with the data stored in PostgreSQL.

## The data
About 10,100 card records and 10,100 customer records, plus a "week 53" file to practise adding a new week of data.

## What I did
- Created a PostgreSQL database and loaded the CSV files with SQL (`CREATE TABLE` and `COPY`).
- Connected Power BI to PostgreSQL.
- Added calculated columns (revenue, age group, income group) and week-over-week measures in DAX.
- Built 3 report pages:
  - **Transaction report:** revenue, interest, transaction count and amount; revenue by quarter, expense type, education, job, card category and chip use.
  - **Customer report:** revenue by income group, age group, marital status, education, dependents, gender and top states; customer satisfaction.
  - **Percentage change:** week-over-week change in revenue, transaction amount and transaction count.

## What I found
- Week over week, revenue went up 28.8%, transaction amount up 35.0% and transaction count up 3.4%.
- Overall revenue was 57M, with 8M in interest and 46M in transaction amount.
- Male customers brought in more revenue (31M) than female customers (26M).
- Blue and Silver cards make up 93% of the total.
- Texas, New York and California bring in 68% of the total.
- The overall activation rate is 57.5%, and the delinquent rate is 6.06%.

## Tools
PostgreSQL, SQL, Power BI, DAX.

## Files
- `Financial Dashboard queries.sql`: the SQL that creates and loads the tables
- `credit_card.csv`, `customer.csv` and the two "addon" files: the data
- `credit card financial report.pbix`: the Power BI file
- `credit card customer report.pdf` and `percentage change.pdf`: PDFs of the pages
- `Customer Report Interactive Dashboard.mp4`: a short screen recording
