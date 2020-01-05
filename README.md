# Analytics-Vidya-India-ML-hiring-hackathon-2019

# Loan Delinquency Prediction

Loan default prediction is one of the most critical and crucial problem faced by financial institutions and organizations as it has a noteworthy effect on the profitability of these institutions. In recent years, there is a tremendous increase in the volume of non – performing loans which results in a jeopardizing effect on the growth of these institutions. 
Therefore, to maintain a healthy portfolio, the banks put stringent monitoring and evaluation measures in place to ensure timely repayment of loans by borrowers. Despite these measures, a major proportion of loans become delinquent. Delinquency occurs when a borrower misses a payment against his/her loan.

Given the information like mortgage details, borrowers related details and payment details, our objective is to identify the delinquency status of loans for the next month given the delinquency status for the previous 12 months (in number of months)

# Data Description

https://datahack.analyticsvidhya.com/contest/india-ml-hiring-hackathon-2019/

# train.zip
train.zip contains train.csv. train.csv contains the training data with details on loan as described in the last section

# Data Dictionary
![image](https://user-images.githubusercontent.com/41851165/66797922-f6832c00-ef29-11e9-8efa-8710c1b08a99.png)

# test.zip
test.zip contains test.csv which has details of all loans for which the participants are to submit the delinquency status - 0/1 (not probability)

# sample_submission.zip
sample_submission.zip contains the submission format for the predictions against the test set. A single csv needs to be submitted as a solution.

# Evaluation Metric
Submissions are evaluated on F1-Score between the predicted class and the observed target.
 
# Public and Private Split
Test data is further randomly divided into Public (40%) and Private (60%) data.
Your initial responses will be checked and scored on the Public data.
The final rankings would be based on your private score which will be published once the competition is over.
Hackathon Rules
Setting the final submission is mandatory. Without a final submission, the submission corresponding to best public score will be taken as final submission
Use of external datasets is not allowed
Use of loan_id variable as an input to the model is not allowed
You can only make 15 submissions per day
Code file is mandatory while setting final submission. For GUI based tools, please upload a zip file of snapshots of steps taken by you, else upload code file.
The code file uploaded should be pertaining to your final submission.
No submission will be accepted after the contest deadline

# Extracting features:
- Convert categorical features to dummy variables.
- Convert dates to Date_Time format and extract features Month, Week, Day of th month, Day of the week.
- Find the feature importances and the correlated features
- Feature importance - Gives what are the features in the data influence the label (here, 1- delequent, 0- non-delequent)
- Correlated features - The features that are correlated to the label are important in classification algorithm (but not in regression algorithm)
- Extracting features like Max delequent of previous months, Min delequent of previous months, Max min diffetence of previous months, Sum of delequent of previous months, Mean delequent of previous months, Variance delequent of previous months, Number of delequent months, Median of delequent of previous months, Skewness of previous months - gives whether the delequency is more in the later or earlier months, Kurtosis of previous months - tailedness - i.e, how the delequency is in recent months


# F1 score = 0.405

### Leaderboard

* **[Public LB](https://datahack.analyticsvidhya.com/contest/india-ml-hiring-hackathon-2019/lb?page=2)** : **398th/712 Rank**
* **[Private LB](https://datahack.analyticsvidhya.com/contest/india-ml-hiring-hackathon-2019/pvt_lb)** : **258th/712 Rank**
