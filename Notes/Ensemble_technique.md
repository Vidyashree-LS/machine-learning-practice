# Ensemble Technique
- It is Ml technique which uses multiplr algorithms to improve the model performance 
1, Bagging
2. Boosting

# when we use Ensemble techniques?
- when decision tree is not performing well then we use ensemble technique 

# Bagging
- it is an ensemble technique which uses 100 decision tree by default and parallely it process all the trees
- we this when desicion tree becomes overfit
- It reduces the variance

# what is Random Forest?
- it is supervised learnng algorithm which comes under bagging ensemble technique and we can use for both regression and classification 

# How RF works?
- step 1: It creates 100 decision trees 
- step 2: It creates random samples for all 100 trees with the help of boot straping sampling technique
- step 3: It parralelly trains all the 100 trees (Tree is independent)
- step 4: how RF predicts the output:
          For calssification it takes majority of all decision results
          for regressio it takes average of all decision tree results

# When not to use RF?
- When Descision Tree is underfit because it is using Bagging it reduces variance not bias
- For larger datasets we should not use Random Forest because it takes more time and depth of the tree will be more

>Syntax: form sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
>        model = RandomForestClassifier(n_estimators = 100)
>        

