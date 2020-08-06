# Will-They-Default

  The main goal of this project is to  predict whether or not customers from a bank will default on their credit card payments, (Not pay their balance).
Defaulting on credit card payment means that a customer has not paid their credit card balance for a certain periiod of time, usually 180 days, the credit issuer assumes you will never pay that debt. The results are that the credit card account gets closed, and the customer's credit score drops dramatically. 

  We will assume that a bank in Taiwan has tasked us with creating a Machine Learning model to predict which customers will or will not default on their credit card payment, as a preventative measure to be able to decide whether or not credit shuold be issued in the first place. The bank has already aqcuired some historical data from t April to September 2005 which includes 24 variables, (23 used for prrediction and the last one is what we want to predict):
  
### Input Variables:

 - LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit
 - SEX: Gender (1=male, 2=female)
 - EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
 - MARRIAGE: Marital status (1=married, 2=single, 3=others)
 - AGE: Age in years
 - PAY_0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)
 - PAY_2: Repayment status in August, 2005 (scale same as above)
 - PAY_3: Repayment status in July, 2005 (scale same as above)
 - PAY_4: Repayment status in June, 2005 (scale same as above)
 - PAY_5: Repayment status in May, 2005 (scale same as above)
 - PAY_6: Repayment status in April, 2005 (scale same as above)
 - BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
 - BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
 - BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
 - BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
 - BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
 - BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)
 - PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
 - PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
 - PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
 - PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
 - PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
 - PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)

### Output Variable:

 - default.payment.next.month: Default payment (1=yes, 0=no)
 
  We will be focusing on visualization and analysis of the data to understand it and derive some interesting conclusions before we even begin to make the model. then we will direct our attention to developing and evaluating the model in AWS Sagemaker Studio, first locally, (in our machines), and then in the Cloud using AWS S3 and Sagemaker. We will also deploy the model iin the cloud and perform inference with it, a process that proveed to be very easy with AWS.
 
 
## Libraries used:

### Data preprocessing and visualization:

  - pandas, numpy, matplotlib, seaborn and sklearn  
  
### Model Training and Evaluation:

  - XGBoost froom xgboost library in python, XGBoost algorithm in Amazon Web Services Sagemaker

### Acknowledgements:

 - This dataset was obtained from kaggle at: https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset

 - Lichman, M. (2013). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

 - The original dataset can be found at the UCI Machine Learning Repository.
 
 - Modern Artificial Intelligence course at https://www.udemy.com/course/modern-artificial-intelligence-applications
 
 - AWS Fundamentals: Going Cloud-Native at https://www.coursera.org/learn/aws-fundamentals-going-cloud-native
