# Predicting NYPD Churn

## Background 

NYC Citywide Payroll Data for each Fiscal Year is publicly accessible via NYC Open Data. The NYC Citywide Payroll dataset covers the Fiscal Years spanning from Fiscal Year (FY) 2017 to FY 2021 and has information about all NYC public employees, including information about their names, data of births, which city agency they work for, their salary, and which city borough they conduct their work in. We are interested in this data for the purposes of predicting whether an employee of the New York City Police Department (NYPD) stops working for the agency within a span of one or two years. Employee turnover can be quite costly for employers, so being able to identify which factors might contribute to employee turnover and predict how much employee turnover there might be in a given fiscal year could aid employers in not only reducing employee turnover but also in efficiently allocating budgetary resources for addressing turnover, which is likely to interest Human Resources (HR) Professionals.

For the purposes of predicting NYPD employee turnover, optimized multiple logistic regression and random forest classifier models were fit to the data.


## Model Fitting and Insights

Compared to a model that simply predicts the majority class (not churned), the logistic regression model that we optimized for the data achieved a classification accuracy of nearly 93 percent that was greater than the null model's classification accuracy of approximately 89 percent by 0.04 points, a difference that a likelihood ratio test suggested was significant. 

Still, the logistic regression model underestimated the amount of churn that occurred during the period examined, predicting that 9 percent of employees churned when 11 percent of employees churned. Underestimating churn is an issue because a HR department relying on an algorithm that underestimates the amount of churn might not have budgeted enough resources to recruit and train new employees. 

The Random Forest Classifier performed similar to the multiple logistic regression model, also underestimating the amount of churn. The variable importance plot of the classifier identified an employee's total compensation and the amount of overtime hours an employee worked as important variables for predicting an employee's likelihood of churning. HR professionals might want to continue to examine an employees pay and the number of hours that they work when seeking to reduce employee turnover. 


## Navigating this repository
The markdown file 'project 1.Rmd' contains all of the code used in the project. The other files in the repository link to the data analyzed in the project
