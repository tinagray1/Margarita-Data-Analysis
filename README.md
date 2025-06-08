# Margarita Data Analysis
## Data analysis project using Excel and Tableau

### Project Overview
Recently, in a company wide meeting, members of corporate revealed that the restaurants will be running a promotion on margaritas every weekend, all day, all summer. The promotion states that regular size margaritas would sell for $5  (discounted from $9) and large margaritas would sell for $8 (discounted from $12).
They justified this by saying alcohol sales have been trending downward, so discounting the drinks will encourage more people to buy them and boost alcohol sales.
I was curious about how they came to this conclusion. I wondered - if I were a data analyst in corporate and they asked me to look into the data to come up with solutions for the downward trend in liquor sales, what would I recommend? Is this promotion the best option, or should we consider something else to drive liquor sales?

### Process Overview
1. Extracting data
   - I downloaded the data in .csv format from our POS system, Toast.
   - Toast limits you to only downloading one month of data at a time. I decided to look at [March 2024](ItemSelectionDetails_2024_03_01-2024_03_31.xlsx), April 2024, June 2024, July 2024, March 2025, and April 2025.
2. Data Cleaning (Excel)
   - Removed columns that were irrelevant to the analysis or redundant to save processing time in SQL and Tableau
   - Added a column using the TEXT function in Excel to convert the full date/time into the day of the week for each transaction.
   - Created pivot tables to get an overview of the data.
   - For the months in 2025, I added an additional table that contained data about the liquor sold with combo deals. Toast bundles combo transactions together in a way that hides the specific items ordered in combos, so I had to extract this data separately to ensure that these combos were accounted for. Combos did not exist in the months of 2024, so I only had to do this for March and April of 2025.
3. Data Visualization (Tableau)
   - Built an interactive dashboard that allows the user to filter the sales data by month.
   - [Click to view dashboard](https://public.tableau.com/app/profile/tina.gray5009/viz/LiquorSalesAnalysis_17493409162170/Dashboard1)

### Key Insights
- When I did my initial calculations in Excel for liquor sales as a percentage of total sales, I saw a very signifcant drop from last year to this year. This is likely what caused corporate to want to take action and run this promotion. Initially, it seemed like % liquor sales had dropped from 9.9% in March 2024 to 7.3% in April 2025. However, I realized that our POS system, Toast, was counting all items in our combo bundle as 'Food', even though each combo comes with a drink. These combos were rolled out in late 2024, so they were only effecting the 2025 data in this case. After accounting for the discount that comes with ordering the combo and all of the liquor that was ordered with combos, I realized that the % liquor sales would have been 8.7% in April 2025. Still a decrease from the previous year, but not as dramatic as it seemed at the start.
- For each month, total liquor sales were always highest on Saturdays.
- Regular size margaritas are being offered at approximately 45% discount and large margaritas are being offered at approximately 32% discount. If we sell approximately the same amount of large and regular size margaritas, we would need a 61% increase in demand for margaritas to break even.
- There is typically only 1 liquor item ordered if a guest buys something off of the liquor menu. Guests ordered only 1 liquor item 12,741 times, while they ordered 2 liquor items only 5,189 times.

## Conclusion/Recommendations
- After performing this analysis, I do not think that the current promotion for discounted drinks on weekends will result in an increase in liquor sales. Needing approximately a 61% increase in liquor sales to break even is too big of a goal. Especially because the promotion discounts drinks on the day that has the largest alcohol sales volume. In addition to this, it will likely not encourage guests to go up and buy another margarita. The restaurant that I analyzed is in an area surrounded by bars, so a majority of guests will likely still only have one drink before moving on to their next location.
- I found that customers can already get margaritas at a discounted rate if they order it with the combo. It seems a little redundant to run this promotion in alongside the combo deal if we are trying to increase liquor profit margins.
- If we want to increase margarita profit margins, we need to either reduce cost of goods sold or increase demand. I think we should roll out new margarita flavors and discountinue the sangrita. Sangritas are the worst performing liquor item, so we can replace them with fun, summery flavors like mango, strawberry, and pineapple. We can flavor the margaritas using syrups that we can order from our suppliers, eliminating the need for any extra prep by our team. Discontinuing the sangrita also means that we no longer have to order red wine. The flavor syrups will be much cheaper than the wine, so this will improve our cost of goods sold. We can push advertisements and coupons out to loyalty members to encourage regular customers to try the new flavors, and the discount is more exclusive. This could encourage more people to sign up for the loyalty program as well in order to get a discounted drink.
