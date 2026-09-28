# PhonePe Transaction Analysis | Power BI

An interactive Power BI project analyzing **300,000 transactions** to explore payment patterns, service performance, transaction outcomes, and user demographics.

## Project Overview

This project uses Power Query for data preparation, DAX for KPI calculations, and Power BI for interactive reporting. The dashboard helps users explore monthly payment trends, compare services, and understand transaction performance.

## Objectives

- Analyze transaction volume, value, and payment success rate.
- Compare performance across service categories.
- Track monthly trends and month-over-month changes.
- Explore user demographics and weekday versus weekend activity.
- Filter results by month and payment status.

## Tools Used

- **Power BI Desktop:** Data modeling and dashboard development
- **Power Query:** Data cleaning and transformation
- **DAX:** KPI measures and month-over-month calculations
- **Excel:** Source data

## Dataset

The workbook contains two worksheets:

| Worksheet | Records with IDs | Description |
|---|---:|---|
| All_Transactions | 300,000 | Transaction amounts, services, payment outcomes, and dates |
| All_Users | 107,658 | User IDs, names, ages, and joining dates |

**Transaction period:** January 1–December 30, 2024  
**Distinct transacting users:** 100,761

### Transaction Fields

- Transaction_ID
- Amount
- User_ID
- Service
- Service Type
- Payment_Status
- Reason
- Date

### User Fields

- User_ID
- Name
- Age
- Join_Date

Record counts exclude blank rows. The total user count differs from the transacting user count because not every listed user appears in the transaction data.

The workbook is used for portfolio analysis. Its original provenance is not documented here, and it should not be treated as an official PhonePe performance dataset.

## Project Workflow

1. Imported the Excel source tables into Power BI.
2. Cleaned and transformed the data using Power Query.
3. Organized transaction, user, and date information for analysis.
4. Used DAX measures to calculate KPIs and month-over-month changes.
5. Built interactive charts, slicers, KPI cards, and a service-type tooltip.

## Dashboard Features

### KPI Cards

- Total transaction value
- Total transactions
- Payment success rate
- Total users
- Month-over-month change in transaction count
- Month-over-month change in transaction value

### Visualizations

- **Monthly trends:** Transaction count and value over time
- **Service performance:** Transaction value by service category
- **User demographics:** Distribution of users by age segment
- **Payment timing:** Weekday versus weekend transaction volume
- **User comparison:** Transaction value by user
- **Service detail:** Tooltip showing transaction count by service type

### Interactive Filters

- Month
- Payment status

## Key Findings

The following results were calculated from the complete source workbook without dashboard filters:

| Metric | Result |
|---|---:|
| Total transactions | 300,000 |
| Successful transactions | 287,993 |
| Success rate | 96.00% |
| Transactions with other status labels | 12,007 |
| Distinct transacting users | 100,761 |
| Weekday transactions | 214,812 (71.60%) |
| Weekend transactions | 85,188 (28.40%) |

- **Loans contributed approximately 72.89% of total recorded transaction value**, the largest share among service categories.
- **Approximately 4.00% of transactions had a status other than Successful**, including Failed, Wrong PIN, Insufficient amount, and Server error.
- **Weekdays accounted for 71.60% of transactions.** This is an aggregate comparison, not a per-day comparison, because there are more weekdays than weekend days.

> Transaction value represents recorded payment amounts, not company revenue. Amount totals include all payment statuses unless filtered. Dashboard results may change with slicer selections.


## Skills Demonstrated

- Data cleaning and transformation
- DAX measures and KPI reporting
- Transaction and user analysis
- Interactive dashboard design
- Communicating findings through visualizations

## Author

**Arpita Shaw**

This is an independent portfolio project and is not affiliated with or endorsed by PhonePe.
