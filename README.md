# Product Marketing Campaign

This dataset contains information from a Portuguese banking institution's marketing campaign. The goal was to predict the likelihood of customers subscribing to a term deposit. The dataset includes the original features along with two additional columns, `probability_of_buying` and `customer_response`, which represent the predicted probability of each customer subscribing to a term deposit and whether a customer has subscribed to the term deposit respectively.

## Data Dictionary

### Column Descriptions

| Column               | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| default              | Has credit in default? (categorical - yes, no or unknown)                   |
| housing              | Has housing loan? (categorical - 'yes', 'no')                                   |
| loan                 | Has personal loan? (categorical - 'yes', 'no')                                  |
| contact              | Contact communication type (categorical - 'telephone', 'cellular')                               |
| month                | Last contact month of year (categorical - 'jan', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'dec')      |
| day_of_week          | Last contact day of the week (categorical - 'mon', 'tue', 'wed', 'thu', 'fri')                                  |
| campaign             | Number of contacts performed during this campaign and for this client       |
| pdays                | Number of days that passed by after the client was last contacted           |
| previous             | Number of contacts performed before this campaign and for this client       |
| poutcome             | Outcome of the previous marketing campaign (categorical - 'success', 'failure', 'nonexistent', 'other')                    |
| emp.var.rate         | Employment variation rate - quarterly indicator                             |
| cons.price.idx       | Consumer price index - monthly indicator                                    |
| cons.conf.idx        | Consumer confidence index - monthly indicator                               |
| euribor3m            | Euribor 3 month rate - daily indicator                                      |
| nr.employed          | Number of employees - quarterly indicator                                   |
| probability_of_buying| Predicted probability of subscribing to a term deposit (numeric - 0-1.00)            |
| customer_response    | Has the client subscribed to a term deposit? (binary - yes, no)                       |
| customer_id          | Unique identifier for each customer (numeric - unique identifier)                                     |


### Further Explanation of the Columns

- **nr.employed**: The "Number of Employees" in a single row represents the total number of employed individuals at the time the data was recorded for that specific entry. This value is a quarterly indicator of the region's overall employment level during that period. It provides context about the labor market conditions at the time of the marketing campaign.
- **euribor3m**: The Euribor (Euro Interbank Offered Rate) 3-Month Rate is the average interest rate at which European banks lend to one another for a three-month period. It is a benchmark for short-term interest rates in the Eurozone and can influence borrowing costs for consumers and businesses.
- **emp.var.rate**: Employment Variation Rate, is a quarterly indicator that measures the percentage change in employment levels compared to the previous quarter. It reflects the labor market's health and can influence consumer confidence and economic activity.
- **cons.conf.idx**: Consumer Confidence Index is the index measures the degree of optimism that consumers feel about the overall state of the economy and their personal financial situation. A higher index indicates greater consumer confidence, which can lead to increased spending and investment.
- **cons.price.idx**: Consumer Price Index is the index measures the average change over time in the prices paid by consumers for a basket of goods and services. It is a key indicator of inflation, reflecting the cost of living and purchasing power.

## Usage

This dataset is ideal for analyzing and predicting customer behavior in marketing campaigns. Insights derived from this data can help marketing teams:

1. **Target potential customers**: Focus on customers with a predicted `probability_of_buying` value greater than the average or those labeled as "yes" in the `customer_response` column.
	
2. **Optimize marketing efforts**: Develop more effective, data-driven strategies to improve campaign performance and ROI. By leveraging the included predictions, teams can streamline marketing activities, enhance personalization, and increase customer engagement.

## Citations

- S. Moro, P. Cortez and P. Rita. *A Data-Driven Approach to Predict the Success of Bank Telemarketing*. Decision Support Systems, Elsevier, 62:22-31, June 2014.
- S. Moro, R. Laureano and P. Cortez. *Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology*. In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimaraes, Portugal, October, 2011. EUROSIS.
