# Supply-Chain-Analytics-Project

 ## Goal
  Demand Forecasting of products
  
  What is Demand Forecasting?
    Demand Forecasting is the art & science of predicting customer’s future demand  for  products.
 
 ## DATASET
 - Source: https://archive.ics.uci.edu/ml/datasets/online+retail
 - Multivariate, Sequential, Time-Series dataset
 - Contains all the transactions occurring between 2010-2011 for a UK-based and registered non-store online retail.
### Correlation
<p align="center">
<img src="https://github.com/Oprishri/Supply-Chain-Analytics-Project/blob/master/images/correlation.PNG" alt="" width="600" height="300" style="vertical-align:top; margin:10px">
 </p>
 
## A Machine-Learning Approach (3- steps Model)

- Data is first clustered (Clustering)
- Output from clustering is then used as labelled(with cluster no.) training data for classification (Classification)
- Then the no. of sales is predicted on the basis of regression model employing ‘cluster no.’ as one of the features. (Prediction)

### CLUSTERING:
 Challenge:
 - Mixed Attributes : Numerical + Categorical
 - Categorical were also important, couldn’t be removed !
 - Converting to numerical would compromise with significance of categorical attributes 
 
Solution:
 - Algorithm which considers mixed attribute : K-Prototypes

**CLUSTERING: k-prototypes


