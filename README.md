This data science activity asks you to perform some analysis on behalf of a fictional client, Acme Health. Acme Health is a health insurance provider that manages several Medicare Advantage plans across the US. They are concerned about member retention and need your help analyzing their data and building a predictive retention model. The assignment uses a combination of real and simulated data.

You can complete the assignment in any open-source language (we mostly use Python and R). Please include clean commented code as well as a write up of your results. This should include a separate code file (with comments and broken out by section) and a word file or PDF containing the write up.

The Data

The client is interested in effect of both individual and community-level predictors on member retention. As such, they have added a new item measuring intent to re-enroll to their standard internal customer survey, which is included in this folder. They have also included a zip code-level data extract from the Social Determinants of Health (SDOH). Additionally, they have appended an internal measure of customer service interaction to each customer record in the survey.

Finally, code books for each data set are included. You will use these to complete the assignment. You will want to begin by familiarizing yourself with these two data sets.

Note that this data is dirty. Some variables may need to be recoded, cleaned, or retyped. Some variables may even be altogether unusable. Preparing this data for analysis in a sensible way is an important part of this assignment.

Part I: Descriptive Statistics/EDA and Data Cleaning

1.	Start by familiarizing yourself with the data. Look at each of the predictors and assess how each is coded as well as the variable’s typing. As noted above, some of the data may be messy, coded in ways that are difficult to analyze or have inappropriate typing. Additionally, some columns may have missing data. Data may be missing at random or according to more meaningful patterns. Use this section to perform any needed data cleaning and assess the missing data across the columns. Be sure to include a paragraph in the write up explaining your process. Feel free to come back to this section if you discover the need for additional data cleaning later in the assignment.
2.	The client is interested in seeing the average median household income and average percentage of the population with a bachelor’s degree, broken down by state. Aggregate the SDOH data to produce a table showing these averages across zip codes by state.


Part II: Merging the Data
Merge the SDOH data into the survey data. Keep in mind, zip codes change regularly and a few zip codes in the survey may not have matches in the SDOH file. Be sure to note any unmatchable zip codes in your write up.


Part III: Inferential Statistics
Before doing any predictive modeling, the client wants a statistical analysis identifying some key relationships in the data. In this section you will perform a regression analysis for the client and extract some key insights.

The dependent variable comes from the survey data: Q9.6_1. In this item, respondents reported how likely they are to re-enroll in their Medicare Advantage plan. You will likely need to recode this variable to perform a regression analysis. When thinking about your plan to recode, consider which type of estimator (e.g., OLS, logit, etc.) you plan to use and recode appropriately.

Next, use the code books to select a subset of key variables that you think may have an important role in explaining re-enrollment. Using all the variables available in the two included data sets would likely be too much for this type of analysis. You may want to perform some additional EDA to inform your choices. Write out hypotheses for some of your key variables. 

Finally, fit a model to the data. Display the model output in a table and provide an interpretation in your write up. What can we learn about the drivers of disenrollment intention from this model? 

Additionally, provide an explanation for why you selected the variables you did, why you selected the estimator and variable coding that you used, how you dealt with missing data, and why you specified the functional form of the model as you did. There is no right or wrong approach here, but we would like to understand your thinking.

Part IV: Predictive Modeling
In addition to the regression analysis, the client wants a predictive model for re-enrollment intention. They would ultimately like to use this model to score their customers who received older versions of the survey without the re-enrollment intention item. Use the data provided to train one or more machine learning models predicting intent to re-enroll. As in Part III, it’s up to you to decide what makes the most sense in terms of recoding the outcome measure.
In the write up briefly explain any choices you made regarding feature engineering, model selection, and model tuning. Additionally, explain your strategy for cross validating the model. If you want, you can train the model using multiple algorithms in order to compare performance across different approaches.
Produce a table along with any relevant figures showing the performance of your model(s). Of the models you produced, which would you recommend the client use?
![image](https://user-images.githubusercontent.com/97277567/203465975-81eeebd0-91a4-4336-bcb5-966b267b3fef.png)
