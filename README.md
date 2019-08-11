# Udacity-Data-Analyst-Project-04---Website-A-B-Test

## Overview
A/B tests are very commonly performed by data analysts and data scientists. Udacity assigned a project based on understand the results of an A/B test run by an e-commerce website. Scenario is a company has developed a new web page in order to try and increase the number of users.

Goal is to find that the new wevsite is performing well or not as compared to the old one. I performed different steps with the data set 
in order to acheive our aim. Steps involved were removing duplicate user ids , page assignment , hypothesis testing and standard statistical tests and multiple regression modelling.

#### Python libraries used:
      1.Numpy
      2.Panadas
      3.Matplotlib.pyplot
      4.Random

#### Data Sets:
      1.ab_data.csv
      2.countries.csv
      


## Progress Outline

#### Part 1 - Probablity
Statistics were performed in order to get the probabilities for conversion regardless of page. Analyzing the data we can predict         the conversion due to a page.

#### Part 2 - A/B Test
Next, hypothesis testing was conducted assuming the old page is better unless the new page proves to be definitely better at a           Type I error rate of 5%.

The data was bootstrapped and sampling distributions were determined for both pages. Conclusions were drawn on conversions for           both pages by calculating p-values.

#### Part 3 - Regression
Logistic regression was then performed to confirm results of the previous steps. Null and alternative hypotheses associated with         this regression model were stated and verified using statsmodel.

Next, along with testing if the conversion rate changes for different pages, I added an effect based on which country a user             lives. Statistical output using logistic regression was provided to check if country had an impact on conversion.


## Conclusion

- The conversion rate for the new page was not superior to that for the old page
- The country of the user did not impact the rate of conversion between the new and old page
