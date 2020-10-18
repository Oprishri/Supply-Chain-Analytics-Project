# Supply-Chain-Analytics-Project

 ## Goal
  Demand Forecasting of products
  
  
    Demand Forecasting is the art & science of predicting customer’s future demand  for  products.
 
 ## DATASET
 
 - Source: https://archive.ics.uci.edu/ml/datasets/online+retail
 - Multivariate, Sequential, Time-Series dataset
 - Contains all the transactions occurring between 2010-2011 for a UK-based and registered non-store online retail.
 - Dataset is used from online retail data of a gift shop.
 - Attributes are InvoiceNo, StockCode, Description, Quantity, InvoiceDate UnitPrice, CustomerID, Country.
### Correlation

<p align="center">
<img src="https://github.com/Oprishri/Supply-Chain-Analytics-Project/blob/master/images/correlation.PNG" alt="" width="600" height="300" style="vertical-align:top; margin:10px">
 </p>
 
### Created new features from text column "Description"

 - Picked out the nouns from every rows using POS tagger for product name and created a new column named Product_type
 - Picked out colour of the product from each rows and created a new column named Colour_type
 
### Created new column revenue
 
 - Revenue = UnitPrice * Quantity
 
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

### CLUSTERING: k-prototypes

- Based on the k-means paradigm
- Works well with mixed data, preserving its efficiency.
- Maximises the intra cluster similarity of objects
- Object similarity measure is derived from both numeric and categorical attributes

### Clustering output:

 The output column from clustering of Train was used as Target variable for classification training set 
 
## CLASSIFICATION: 

 To build model for cluster classification
 Linear SVM of machine learning algorithm performed very well.
 
 ## Prediction of demands
 
  - Collected all features together and mark "Quantity" column as a target variable.
  - Splitted the whole dataset into train test and predicted the quantity of the items
  - Demand forecasting of quantity column, the machine learning algorithm random forest performed very well.

## Conclusion

- The data pre-processing phase facilitates the formation of the inputs to the models.
- The feature engineering process helps create new variables that bring additional value to demand interpretation.
- The three-step model involving clustering, classification and prediction enables the company further to visualize the relationship between predictor variables and customize the forecasting approaches accordingly.







