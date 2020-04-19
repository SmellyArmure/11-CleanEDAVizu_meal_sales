_________________________________
|                                                                           |
|          CleanEDAVizu (meal_sales)             |
|________________________________|

My own EDA of the dataset given in the following TDS article: 

Explore and Visualize a Dataset with Python
Or how to learn to create beautiful and insightful graphs with Python — a code-along guide
by F. Bosler, Aug, 31, 2019

Summary of the graphs in the notebook:
1. Conversion rate development
	Rolling conversion rate average on 60 days through time from 2014 to 2019
2. Conversion rate accross sales reps
	histogram (distribution) of the number of sales reps by class of conversion rate
3. Effect of number of accounts
	facetgrid of kdeplots (density distribution) of the conversion rates for each number of accounts of sales reps
4. Effect of meals
	barplot of frequency (pct) of conversion depending on the type of meal
	barplot of frequency (pct) of conversion depending on the delay with order
	heatmap of frequency of meals (pct) depending of  type of meal / cat of price / delay with order

Recap of the Situation:

You are tasked with figuring out how to increase your sales team’s performance. In our hypothetical situation, potential customers have rather spontaneous demand. When this happens, your sales team puts an order lead in the system. Your sales reps then try to get set up a meeting that occurs around the time the order lead was noticed. Sometimes before, sometimes after. Your sales reps have an expense budget and always combine the meeting with a meal for which they pay. The sales reps expense their costs and hand the invoices to the accounting team for processing. After the potential customer has decided whether or not they want to go with your offer, your diligent sales reps track whether or not the order lead converted into a sale.

For your analysis, you have access to the following three data sources:

    order_leads (contains all the order leads and conversion info)
    sales_team (includes companies and responsible sales reps)
    invoices (provides information on the invoices and participants)
