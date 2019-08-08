# Udacity-Data-Analyst-Project-04---Website-A-B-Test

## Overview
A/B tests are very commonly performed by data analysts and data scientists. Udacity assigned a project based on understand the results of an A/B test run by an e-commerce website. Scenario is a company has developed a new web page in order to try and increase the number of users.

Goal is to find that the new wevsite is performing well or not as compared to the old one. I performed different steps with the data set 
in order to acheive our aim. Steps involved were removing duplicate user ids , page assignment , hypothesis testing and standard statistical tests and multiple regression modelling.

#### Data Sets:
      1.ab_data.csv
      2.countries.csv
      


## Progress Outline

#### Part 1 - Probablity
Statistics were performed in order to get the probabilities for conversion regardless of page. Analyzing the data we can predict the conversion due to a page.

#### Part 2 - A/B Test
Next, hypothesis testing was conducted assuming the old page is better unless the new page proves to be definitely better at a Type I error rate of 5%.

The data was bootstrapped and sampling distributions were determined for both pages. Conclusions were drawn on conversions for both pages by calculating p-values.

#### Part 3 - Regression
Logistic regression was then performed to confirm results of the previous steps. Null and alternative hypotheses associated with this regression model were stated and verified using statsmodel.

Next, along with testing if the conversion rate changes for different pages, I added an effect based on which country a user lives. Statistical output using logistic regression was provided to check if country had an impact on conversion.


## Conclusion

#### Part 1 - Probablity
- The probability of an individual converting regardless of the page they receive is 11.96%.
- If the individual was in the control group, the probability they converted is 12.04%.
- If the individual was in the treatment group, the probability they converted is 11.88%.
- By the result provided above, we can say thay both the pages have similar performance. So we cannot state that one page leads to more   hits.

#### Part 2 - A/B Test
- Z-score : 1.3109241 is less than the critical value of 1.959963. Hence we can conclude it as null hypothesis.
- We find that old pages performs a bit well.

#### Part 3 - Regression
- For a unit increase in a_page, conversion is 1.08 % more likely to happen
- We can imply that coefficient of variable "US_ab_page" and "CA_ab_page" are different from the coefficient of ab_page itself.
- Conversion is 1.03 times likely to happen for US and ab page users than UK and ab page users.
- Conversion is 1.08 times likely to happen for CA and ab page users than UK and ab page users.
- Convert is 0.5 % likely to happen for the users in US than UK.
- Convert is 1.01 % likely to happen for the users in US than UK
