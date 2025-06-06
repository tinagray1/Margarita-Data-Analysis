# Margarita Data Analysis
## Data analysis project using Excel, SQL, and Tableau

### Project Overview
Recently, in a company wide meeting, members of corporate revealed that the restaurants will be running a promotion on margaritas every weekend all summer.
They justified this by saying alcohol sales have been trending downward, so discounting the drinks will encourage more people to buy them and boost alcohol sales.
I was curious about how they came to this conclusion. I wondered - if I were a data analyst in corporate and they asked me to look into the data to solve the issue of alcohol sales in the summer, what would I recommend? Is this promotion the best option, or should we consider something else to drive liquor sales?

### Process Overview
1. Extracting data
   - I downloaded the data in .csv format from our POS system, Toast.
   - Toast limits you to only downloading one month of data at a time. I decided to look at March 2024, April 2024, June 2024, July 2024, March 2025, and April 2025.
2. Data Cleaning (Excel)
   - Removed columns that were irrelevant to the analysis or redundant to save processing time in SQL and Tableau
   - Filtered data to remove rows that contained customer phone numbers
   - Added a column using the TEXT function in Excel to convert the full date/time into the day of the week for each transaction.
   - Created pivot tables to get an overview of the data.
   - For the months in 2025, I added an additional table that contained data about the liquor sold with combo deals. Toast bundles combo transactions together in a way that hides the specific items ordered in combos, so I had to extract this data separately to ensure that these combos were accounted for. Combos did not exist in the months of 2024, so I only had to do this for March and April of 2025.
4. Data Exploration (SQL)
5. Data Visualization (Tableau)

### Key Insights
