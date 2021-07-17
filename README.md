# Blockchain-Governance-Project

# Methodology

## Introduction
In the prior round of modeling governance data, we attempted to use multiple linear regression to determine whether or not there was a meaningful relationship between governance variables and the corresponding ICO size. There were many problems with this approach; however, the most salient problem was that we were comparing categorical variables (governance type, determined qualitatively) against numerical values (ICO Size, Value Creation, Market Cap). In addition, we attempted to use multiple regression models, which may have introduced confounding variables. Therefore, we foresee two key changes for the second iteration of modeling.
It is important to remember our fundamental question: to what extent does governance impact long-term value creation? From this question, two logical forms of analysis arise as key applications.

## Data Recategorization and Visualization
First, we will classify all input governance data values on a discrete scale, ranging from 1 (least centralized) to four (most centralized). We will then classify all ICO Size values on a discrete scale as well, ranging from 1 (small) to 4 (extremely large). This way, we will ensure we are comparing across categorical classifications. We will then visualize ICO Size against each of these governance input values. This should give us a strong inclination towards the shape of the data, its relative skewness / kurtosis, and what analysis makes the most sense moving forward. 

## Conditional Probability
In this part we will create a table in which the x axis ranges from least to most centralized for a given governance value and the right axis ranges from least to most successful for a given quality metric. We will then place the counts of all instances occurring in each block of the table; therefore, this table will allow us to discern the probability of any characteristic either being a success or a failure. After each table, we will list the three most important values whose conditional probabilities suggest a correlation with success.

## Linear Regression
Finally, we will run regression analysis between each dependent variable and ICO Size. If necessary, we will log-normalize the data again. This should give us the ability to determine correlation between each individual variable and ICO size. We will again rank the importance of each variable (ranking its correlation coefficient versus its standard error) and determine the three variables which most closely impact ICO size. We will then compare these variables to our results from the conditional probability section. If they are the same, we conclude our results with the most significant variables. If they are not, we should modify our original methodology with more advanced statistical methods backed by concrete explanations.

## Statistical Analysis
Per Dr. Ali Nejadmalayeri’s recommendations, we should also run a series of statistical variables analyzing the shape and error metrics of this data. For our initial analysis, I recommend the following three metrics:
<ul>
  <li>Skewness</li>
  <li>Kurtosis</li>
  <li>Downside risk between ICO size and centralization/li>
</ul>

## Deliverables
Our deliverable, to be delivered to Alan on behalf of the BRI will be a GitHub repository containing the following:
<ul>
  <li>The original dataset</li>
  <li>The cleaned and modified dataset</li>
  <li>Data visualization</li>
  <li>Conditional probability tables and results</li>
  <li>Linear regression analysis</li>
  <li>Additional statistical analysis</li>
</ul>
