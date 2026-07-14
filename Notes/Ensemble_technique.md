# Ensemble Technique
- It is Ml technique which uses multiplr algorithms to improve the model performance 
1, Bagging
2. Boosting

## when we use Ensemble techniques?
- when decision tree is not performing well then we use ensemble technique 

# Bagging
- it is an ensemble technique which uses 100 decision tree by default and parallely it process all the trees
- we this when desicion tree becomes overfit
- It reduces the variance

# what is Random Forest?
- it is supervised learnng algorithm which comes under bagging ensemble technique and we can use for both regression and classification 

### How RF works?
- step 1: It creates 100 decision trees 
- step 2: It creates random samples for all 100 trees with the help of boot straping sampling technique
- step 3: It parralelly trains all the 100 trees (Tree is independent)
- step 4: how RF predicts the output:
          For calssification it takes majority of all decision results
          for regressio it takes average of all decision tree results

### When not to use RF?
- When Descision Tree is underfit because it is using Bagging it reduces variance not bias
- For larger datasets we should not use Random Forest because it takes more time and depth of the tree will be more

>Syntax: form sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
>        model = RandomForestClassifier(n_estimators = 100)

### Para
max_samples = 0.8
- by using this parameter we can assign random parameters to all the trees

-----------------------------------------------------------------------------------------

# Boosting
- It is an ensembling echique which uses multiplt decision trees which is used for both regression and classifcation
- We use boosting when decision tree become underfit (it reduces the bias)
- Sequentially it process all 100 trees (Trees are dependent because the second model corrects hte mistakes of previous models)

# XGBoost
- XGBoost stands for Extreme Gradient Boosting Algorithm hwich comes undeer boosting ensemble technique 

### Techniques which uses internally
1. Regularization
2. Gradient Descent

### Advantages of XGBoost
- Scaling techniques not required 
- It handles missing values
- It handles categorical columns
- It works well with large dataset
- It handles both high variance and high bias

### How it works
1.  


