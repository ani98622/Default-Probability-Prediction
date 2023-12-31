# Default-Probabilty-Prediction
**Objective** :  To predict the *probability* that a customer/individual does not pay back their credit card balance <br>&emsp;&emsp;&emsp; amount in the *future* based on their monthly customer profile. The target binary variable is calculated <br>&emsp;&emsp;&emsp; by observing 18 months performance window after the latest credit card statement, and if the <br> &emsp;&emsp;&emsp; customer does not pay due amount in 120 days after their latest statement date it is considered a <br>
&emsp;&emsp;&emsp; default  event.;

**Data sets** : There are a total of three *normalized* data sets namely -<br>
&emsp;&emsp;&emsp;1 - test_data.feather (2.74 GB) - corresponding test data and objective is to predict the target label <br>
&emsp;&emsp;&emsp; for each 'customer_ID' <br>
&emsp;&emsp;&emsp;2 - train_data.feather (1.33 GB) - training data with 'multiple statement dates' per customer_ID <br>
&emsp;&emsp;&emsp;3 - train_labels.csv (29.3 MB) - target 'label' for each 'customer_ID' <br>

**Variable Description** :<br>
&emsp;&emsp;&emsp;D_* = Delinquency variables <br>
&emsp;&emsp;&emsp;S_* = Spend variables <br>
&emsp;&emsp;&emsp;P_* = Payment variables <br>
&emsp;&emsp;&emsp;B_* = Balance variables <br>
&emsp;&emsp;&emsp;R_* = Risk variables <br>

**_Note_** : Some of the variable/predictors are of categorical type -<br>
&emsp;&emsp;&emsp;['B_30', 'B_38', 'D_114', 'D_116', 'D_117', 'D_120', 'D_126', 'D_63', 'D_64', 'D_66', 'D_68']<br>

**Output** : The result of the model has to be provided as a csv file in the format which contains only 'two columns' as :<br>
&emsp;&emsp;&emsp; | Customer_ID  |  Probabilty |  <br>
