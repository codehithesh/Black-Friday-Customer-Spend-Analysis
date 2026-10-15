# Walmart - Confidence Interval and CLT Case Study

### About Walmart

Walmart is an American multinational retail corporation that operates a chain of supercenters, discount departmental stores, and grocery stores from the United States. Walmart has more than 100 million customers worldwide.


### Business Problem

The Management team at Walmart Inc. wants to analyze the customer purchase behavior (specifically, purchase amount) against the customer’s gender and the various other factors to help the business make better decisions. They want to understand if the spending habits differ between male and female customers: Do women spend more on Black Friday than men? (Assume 50 million customers are male and 50 million are female).


### Dataset

The company collected the transactional data of customers who purchased products from the Walmart Stores during Black Friday. The dataset has the following features:

Dataset link: [Walmart_data.csv](https://d2beiqkhq929f0.cloudfront.net/public_assets/assets/000/001/293/original/walmart_data.csv?1641285094)

* User_ID:  User ID
* Product_ID: Product ID
* Gender: Sex of User
* Age:  Age in bins
* Occupation: Occupation(Masked)
* City_Category:  Category of the City (A,B,C)
* StayInCurrentCityYears: Number of years stay in current city
* Marital_Status: Marital Status
* ProductCategory:  Product Category (Masked)
* Purchase: Purchase Amount


### What good looks like?
1. Import the dataset and do usual data analysis steps like checking the structure & characteristics of the dataset.
2. Detect Null values & Outliers (using boxplot, “describe” method by checking the difference between mean and median, isnull etc.)
3. Do some data exploration steps like:
    * Tracking the amount spent per transaction of all the 50 million female customers, and all the 50 million male customers, calculate the average, and conclude the results.
    * Inference after computing the average female and male expenses.
    * Use the sample average to find out an interval within which the population average will lie. Using the sample of female customers you will calculate the interval within which the average spending of 50 million male and female customers may lie.
4. Use the Central limit theorem to compute the interval. Change the sample size to observe the distribution of the mean of the expenses by female and male customers.
    * The interval that you calculated is called Confidence Interval. The width of the interval is mostly decided by the business: Typically 90%, 95%, or 99%. Play around with the width parameter and report the observations.
5. Conclude the results and check if the confidence intervals of average male and female spends are overlapping or not overlapping. How can Walmart leverage this conclusion to make changes or improvements?
6. Perform the same activity for Married vs Unmarried and Age
    * For Age, you can try bins based on life stages: 0-17, 18-25, 26-35, 36-50, 51+ years.
7. Give recommendations and action items to Walmart.

### Evaluation Criteria
1. Defining Problem Statement and Analyzing basic metrics (10 Points)
    1. Observations on shape of data, data types of all the attributes, conversion of categorical attributes to 'category' (If required), statistical summary
    2. Non-Graphical Analysis: Value counts and unique attributes
    3. Visual Analysis - Univariate & Bivariate
        * For continuous variable(s): Distplot, countplot, histogram for univariate analysis
        * For categorical variable(s): Boxplot
        * For correlation: Heatmaps, Pairplots
2. Missing Value & Outlier Detection (10 Points)
3. Business Insights based on Non- Graphical and Visual Analysis (10 Points)
    * Comments on the range of attributes
    * Comments on the distribution of the variables and relationship between them
    * Comments for each univariate and bivariate plot
4. Answering questions (50 Points)
    1. Are women spending more money per transaction than men? Why or Why not? (10 Points)
    2. Confidence intervals and distribution of the mean of the expenses by female and male customers (10 Points)
    3. Are confidence intervals of average male and female spending overlapping? How can Walmart leverage this conclusion to make changes or improvements? (10 Points)
    4. Results when the same activity is performed for Married vs Unmarried (10 Points)
    5. Results when the same activity is performed for Age (10 Points)
5. Final Insights (10 Points) - Illustrate the insights based on exploration and CLT
    * Comments on the distribution of the variables and relationship between them
    * Comments for each univariate and bivariate plots
    * Comments on different variables when generalizing it for Population
6. Recommendations (10 Points)
    * Actionable items for business. No technical jargon. No complications. Simple action items that everyone can understand

### Disclaimer
This analysis is based on the data provided and reflects the state of the dataset as of the time of the analysis. The insights and recommendations are derived solely from my point of view and the dataset in question do not necessarily represent the broader operations or circumstances of the company. The analysis assumes the accuracy of the data as received and has not been independently verified. Future analyses may yield different insights as new data becomes available or as business conditions change.

### Note on Results
Due to the large volume of results generated by this analysis, only a subset has been presented here to illustrate the key trends and patterns. Specifically, the top 10 to 15 results have been included as screenshots to provide a snapshot of the most relevant findings. For a complete view of the data and to explore additional insights, please refer to the full dataset.