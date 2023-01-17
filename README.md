# Loan Default Prediction

![](https://i.imgur.com/pWBEwXX.png)

<h2>Problem statement</h2>
Over the years, So & So Lending Club has been experiencing increase in the dollar amount of loan defaults. The chart above shows the gravity of the problem the company face. As of 2013, the total loan portfolio amounted to $182 million and $30.4 million of that is in default. The situation is getting worse, and requires drastic measures to reverse the trend. 
<br></br>
In this project, I attempted to use machine learning to help So & So Lending Club predict the likelihood of a loan default, and also to identify the factors that driving loan default.

<h2>Languages and Libraries Used</h2>

- R programming language 
- [List of libraries](https://github.com/graphshade/loan_default/blob/main/renv.lock)

<h2>Environment Used </h2>

- <b>Ubuntu 22.04.1 LTS</b>


<h2>Key Findings:</h2>

1. The amount of installment significantly influences the default rate. Thus, the probability of default is 30% and above when the installment amount is above $400 

2. There is a linear relationship between interest rate and likelihood of default. Higher interest rates increase the likelihood of default. Concretely, default rate is above 13% for interest rates starting from 12%

3. Loan defauls for last payment amounts below $6000 is high. In fact,loan defaults go above 40% for last payments between $4000 - $5000. For last payments beyond $6000, loan default drops significantly. Investigating this further, we noticed that these borrowers have longer term loans and may suffer from loan payment fatigue and end up defaulting

4. Lastly, higher loan amounts increase the likelihood of default. The default rate is between 22% to 29% for loan amounts between $10,000 to $30,000

<h2>Recommendations:</h2>

Based on the findings, the following recommendations were made:
1. Operate the model at the 50% predictive probability of default threshold. At this level, the selected model can identify 63% of loan default cases. Historically, this could saved $3 million in loan defaults.This saving in loan default is computed without taking into consideration the cost of associated with wrongly classifying a non-default loan as default. Specifically, operating at the 50% threshold results into wrongly classing 9 out of every 100 observations

2. The customer service department may use the predicted probability of default to segment borrowers and device an outreach campaign targeted at the various segments. For instance, for customers with high probability of default, the customer service department may constantly follow up to understand their financial situation and help them restructure their payment plan

<h2>Reproducing the Analysis:</h2>

<p align="left">

1. [Install R and RStudio](https://techvidvan.com/tutorials/install-r/)
 
2. Clone the project: Run this from the command line
 
 ```commandline
 git clone https://github.com/graphshade/loan_default.git
 ```
 
3. Install Required Libraries Using Virtual Environment: 
   
   You may install the libraries directly on your computer however, using the virtual environment library `renv`. [Follow this guide to install renv](https://www.youtube.com/watch?v=yc7ZB4F_dc0)
   1. Open the app.R file in RStudio
   2. In the RStudio console run `renv::init()` to initiate the renv virtual environment and install the required libraries from the [renv.lock](https://github.com/graphshade/loan_default/blob/main/renv.lock) file 
