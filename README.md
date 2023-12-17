# Capstone_project
 Predicting USA Insurance premiums 

Author: Tisa Yip

## Overview

Multi linear regression analysis of Insurance health premiums in the USA.


## Business Problem

This information could be used to predict the cost of health insurance for an adult living in the USA.

## Data Understanding

The data used in this analysis is from Kaggle <a href=https://www.kaggle.com/datasets/sridharstreaks/insurance-data-for-machine-learning/data> <br>The dataset was created using a script that generated a million records of randomly sampled data points, ensuring that the data represented the population of insured individuals in the USA. 

## Data Modeling

<br><li>Pair plot of the raw data. From the histograms of Age and BMI - you can see the data is uniform in nature.<br>
Children is categorical and charges is fairly normally distributed 
</li>
<img src="https://github.com/xSTILETTOx/Capstone/blob/main/pairplot.png" alt="Alt text" style="max-width: 100%;">

<br><li>QQ-Plot of raw data</li><br>
<li>This QQ plot is strange. There are strong outliers and is showing uniformity in the data</li>
<img src="https://github.com/xSTILETTOx/Capstone/blob/main/RawQQ.png" alt="Alt text" style="max-width: 100%;">

<br><li>QQ-Plot of dummied data</li><br>
<li>Adding dummy variables has improved the qq plot</li>
<img src="https://github.com/xSTILETTOx/Capstone/blob/main/dummiesQQ.png" alt="Alt text" style="max-width: 100%;">

<br><li>QQ-Plot of log transformed data</li><br>
<li>log transforming the continuous variables has altered the qq plot very little compared to the added dummies qq plot</li>
<img src="https://github.com/xSTILETTOx/Capstone/blob/main/logQQ.png" alt="Alt text" style="max-width: 100%;">

<br><li>MSE and R-Squared</li><br>
<li>As you can see the Mean squared error and R-squared improved significantly between the raw and dummied data.</li> 
<li>It had a tiny affect between the dummied data and log transformed data</li>
<li>The train MSE and test MSE are very close in the log transformed data. The model fits well</li>
<li>The R2 = 0.88 which would imply that 88% of the target variance can be explained by the model features. This is significant</li>
<img src="https://github.com/xSTILETTOx/Capstone/blob/main/MSEandR2.png" alt="Alt text" style="max-width: 100%;">