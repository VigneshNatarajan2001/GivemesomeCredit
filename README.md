# GivemesomeCredit
code has been written in python for the following case

Training data has been taken for data exploration to find the missing values and outliers.

TREATING MISSING VALUES
The columns Monthly income and Number of Dependents has missing values.
From analysis it is inferred that the people who has missing income has higher debt ratio. so the mean value of people who has debt ratio greater than 1 has been used to fill the null values in MonthlyIncome column. in the similar way Numberod dependent values are found and filld with the majority value of 0.

TREATING OUTLIERS
From analysing the data the columns "NumberOfTime30-59DaysPastDueNotWorse", "NumberOfTime60-89DaysPastDueNotWorse", "NumberOfTimes90DaysLate" has srong correlation. so I decided to treat all 3 columns together and found out that tha outliers contribute around 50% of the data and decide not to omit the outliers as most of the data will be omitted

"NumberOfTimes90DaysLate" column has been analysed and found out that the outliers contribute only 0.17% to the data and has been omitted 

the initial model is buit using Random forest classifiers and randomized searchCV is used to tuning the hyperparameters. the training accuracy came around 94% and the test accuracy came around 93.5%

the second model used is XGboost and hyperparameter have not been tuned, but the accuracy came around 94% CODE HAVE ALSO GIVEN TO TUNE THE HYPERPARAMETERS FORxgbOOST. PLEASE UNCOMMENT TO RUN THE CODE.


TO RUN CODE:
TO RUN THE .PY FILE PLEASE PROVIDE THE FILE PATH.
