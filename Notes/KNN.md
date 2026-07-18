# what is KNN?
- It is supervised learning algorithm which is used for bith classification and regression
- It uses distance formula(euclidean, manhattan) to predict the output
- It is a lazy algorithm, during model training it judt stores the data
- when we have more feature columns it uses manhattan formula

-step 1: Stores the data
| Feature 1 | Feature 2 | Target |
|-----------|-----------|--------|
| 1 | 100 | 100 | = 29.68
| 7 | 50 | 200 | = 26.92
| 15 | 25 | 300 |  = 50.03       
| 8 | 25 | 400 |  = 50.80
| 9 | 10 | 500 | = 65.49

- step 2: When the new input comes it calculates the distance
- step 3: Then is sorts by ascending order
- Step 4: selcts the top k values 
- step 5: for regressor it takes average, for classifer it takes majority.

- the answer for the aove example is 200 because it takes 

