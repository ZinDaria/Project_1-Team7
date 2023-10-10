# Project 1: Credit Card Fraud Detection
In this project, we analyzed a dataset containing credit card transactions. The main objectives were:

Analyzing credit card transactions occurring over a 2-day period in the accounts of customers from 7 banks in the United Kingdom.
Identifying patterns in fraud versus non-fraud transactions.
Establishing relationships between various data points such as age, gender, transaction type (POS, Online, ATM), transaction time, country of transaction, shipping address, etc.
### Assumptions
All transactions are from customers' accounts domiciled in the United Kingdom, with time zone set to British Summer Time (BST) and amounts stated in Great British Pounds (£).
Individuals aged 30 to 50 are assumed to be more attractive targets for fraudsters due to their greater financial resources.
### Limitations
The data provided, and thus our analysis, is based on 2 specific days of the week (Tuesday and Wednesday).
The data is from 2020 and may not be the most recent available.
### Analysis
*Step-by-step processes are detailed within the Jupyter notebook.

We aimed to answer the following questions:

What age group and gender are most affected by fraud?
Which country is the source of most fraud?
During which time of the day do most fraudulent transactions occur?
After pre-processing the data, a total of 99,977 credit card transactions remained for further analysis. Out of these, 7,192 were fraud transactions, accounting for 7.19% of the total transactions.

The total amount lost to fraud was £459,495 out of a total transaction amount of £11,255,404, making up 4.08% of the total amount. Individual fraud amounts ranged from £5 to £400.

Our analysis revealed the following:

A significant gender gap in victims of credit card fraud, with males at 59.4% and females at 40.6%.
The age breakdown reveals a peak susceptibility among individuals aged 30-50 (4682 cases), followed by those 50-65 (1801 cases), under 30 (572 cases), and 65-90 (137 cases).

An interesting hypothesis arises: the higher incidence among the 30-50 age group might be tied to their potentially higher incomes. Investigating this correlation could enhance our preventive strategies, considering both demographics and economic factors.

The country that ranked highest in originating fraud transactions was the United States at 25.4%. However, the 3 other countries were not far behind, with India at 24.6%, China and Russia at 24.3% and 24.1% respectively. Only 1.7% of the fraud transactions came from the UK where the data was obtained. From this data, credit card fraud transactions are more successful when the origin country is different from the customer's country of residence.

100% of transactions that occurred between 12:00 AM and 6:00 AM were found to be fraudulent. There are two peaks of fraud during the day: 12:00 AM - 6:00 AM and at 1:00 PM.

The percentage of the amount of fraud transactions compared to total transactions amount after 6:00 AM is lower than the percentage of the fraud transaction count compared to total transaction count for the same time of the day, which could mean that on average, fraud transactions are of a lower value than other transactions.

These findings lay the groundwork for improving fraud detection and implementing targeted preventive measures.

### References

Data for this dataset was obtained from  https://www.kaggle.com/datasets/anurag629/credit-card-fraud-transaction-data/data and is intended for learning and exploratory purposes only.

Other sources and their use in this notebook:
Working with secondary axis:
 - https://saturncloud.io/blog/how-to-format-secondary-yaxis-in-pandas/#:~:text=In%20Pandas%2C%20we%20can%20create,format%20and%20customize%20as%20needed
 - https://samchaaa.medium.com/how-to-plot-two-different-scales-on-one-plot-in-matplotlib-with-legend-46554ba5915a
Merging legends for several x-axis charts:
 - https://stackoverflow.com/questions/5484922/secondary-axis-with-twinx-how-to-add-to-legend
 - https://stackoverflow.com/questions/5484922/secondary-axis-with-twinx-how-to-add-to-legend
Setting label per each line: https://stackoverflow.com/questions/64111555/get-lines-and-labels-from-matplotlib-axes
Switching column to a row: https://www.w3resource.com/pandas/dataframe/dataframe-pivot.php
Create the stacked bar chart: https://www.geeksforgeeks.org/create-a-stacked-bar-plot-in-matplotlib/
Working with a string:
 - https://www.softwaretestinghelp.com/python/python-string-split/
 - https://buzzcoder.gitbooks.io/codecraft-python/content/string/loop-through-a-string.html
Mode calculation: https://stackoverflow.com/questions/50208007/calculate-mode-of-a-column-in-pandas-using-other-column-with-same-row-values
Merging by index: https://stackoverflow.com/questions/40468069/merge-two-dataframes-by-index      
Sharing of the same colour for item per different charts: https://github.com/geopandas/geopandas/issues/1269
Adjust spacing between subplots: https://www.geeksforgeeks.org/how-to-set-the-spacing-between-subplots-in-matplotlib-in-python/
How to build Venn diagram:
- https://www.geeksforgeeks.org/how-to-create-and-customize-venn-diagrams-in-python/
- https://stackoverflow.com/questions/19841535/python-matplotlib-venn-diagram
Grouped bar charts: https://www.pythoncharts.com/matplotlib/grouped-bar-charts-matplotlib/
The text annotation for each bar with numbers: https://www.pythoncharts.com/matplotlib/grouped-bar-charts-matplotlib/
Colors set: #https://matplotlib.org/stable/gallery/color/named_colors.html (edited)

### Acknowledgments
Shout out to fellow contributors to this project:

Daria Z.
Neha S.
Seeke O.D
Valentyna K.
It has been great working and learning with you all.
