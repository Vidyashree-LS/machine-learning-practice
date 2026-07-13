# Decision Tree
- It is a supervised learning algorithm which is used for both regression and classifcation 
- It makes the prediction by asking series of questions

# Advantgaes of decision tree
- It handles non-linear data 
- It hanles mixed column types like categorical and numerical columns
- Scaling techniques are not required 

# Disadvantage of Dedcision Tree
- We will not use this decision tree in real time why because, it will become overfit

* Root Node
* Sub or internal node
* leaf node
* split
* purity & impurity

                                     feature name --->root node
                                       /    \ ----->split(always 2)
                          feature                       feature ----->Internal node
                           /\                              /\
                  feature     feature           feature            feature
                    /\          /\               /\                 /\
            label   label   label   label   label   label     label      label --->leaf node or target node


* Example:
|   Feature 1               | fewature2 |   feature 3        |  Target  |
|---------------------------|-----------|--------------------|----------|
|Are you going for lunch?   |   money   |   veg or non-veg   |   Food   |

                                                                    feature 1
                                                               (yes) /        \ (No)
                                                     feature 2                    get Back to wprk
                                                (<=100)/     \ (>100)
                                feature 3                                  feature 3
                            (veg)/ \ (non veg)                           (veg)/  \(non veg)
                    veg biriyani     chicken fried rice         mushroom curry      Chicken Biriyani

# Parameters
# Criterion
- it helps to selct the best node
- it has two values entropy snd gini
- it tskeg the help of hypertuning psrsmeter to slect ehich vslue is the best

# splitter
- It helps to select the best split
- it has two values best and random
- best uses criterion to find the best splitter

# max_depeth
- Default value is none
- we can use integer values instead of none
- It controls the the depth of the tree we use this when we have more number of samples

# min_samples_split 
- min_samples_split = 2 | int
- it checks whether node contains minimum 2 samples or not

# min_samples_leaf
- min_samples_leaf = 1 | int
- It checks whether the leaf node conatins minimum (1) samples or not 

* if any one condition is invalid the entire split is invalid






