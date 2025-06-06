# Margarita-Data-Analysis
## Data analysis project using Excel, SQL, and Tableau

### Project Overview
Recently, in a company wide meeting, members of corporate revealed that the restaurants will be running a promotion on margaritas every weekend all summer.
They justified this by saying alcohol sales tend to trend downward in the summer, so discounting the drinks will encourage more people to buy them and boost alcohol sales.
I was curious about how they came to this conclusion, and wondered - if I were a data analyst in corporate and they asked me to look into the data to solve this issue, what would I recommend? Is this promotion the best option, or should we consider something else to drive liquor sales?

### Process Overview
1. Extracting data
   - I downloaded the data in .csv format from our POS system, Toast.
   - Toast limits you to only downloading one month of data at a time. I decided to look at March 2024, April 2024, June 2024, July 2024, and March 2025.
2. Data Cleaning (Excel)
   - Removed columns that were irrelevant to the analysis or redundant to save processing time in SQL and Tableau
   - Filtered data to remove rows that contained customer phone numbers
   - Added a column using the TEXT function in Excel to convert the full date/time into the day of the week for each transaction.
   - Created pivot tables to get an overview of the data.
4. Data Exploration (SQL)
5. Data Visualization (Tableau)

### Key Insights
