# Column Transformer
- It is a ML technique which combines multiple preprocessing and executes parallely 
- In column Transformer we use only preprocessing techniques not an algorithm
> syntax: from sklearn.compose import ColumnTransformer
>         preprocessing = ColumnTransformer(
>           transformers = [
>               ('name of the preprocessing", preprocessing, col_names)
>               (.....................................................)
>           ],
>           remainder = 'drop' | 'passthrough'
>         )

- example:
preprocessing = ColumnTransformer(
    transformers = [
        'minmax_scaling', MinMaxScaler(), ['f1', 'f2'],
        'robust_scaling', 'RobustScaler(), ['f3', 'f4'],
        'encoder', 'TargetEncoder(), ['f5', 'f6']
        ]
)
xtrain_new = preprocessing.fit_transform(xtrain)

* remainder default value is drop, it drop thr remaining columns
- example:
preprocessing = ColumnTransformer(
    transformers = [
        'minmax_scaling', MinMaxScaler(), ['f1', 'f2'],
        'robust_scaling', 'RobustScaler(), ['f3', 'f4'],
        ],
        remainder = 'drop'
)
xtrain_new = preprocessing.fit_transform(xtrain)
* here the xtrain will onlu have 4 columns because the reamining colimns are dropped


* Remainder is pass through it keeps the remaining columns
preprocessing = ColumnTransformer(
    transformers = [
        'minmax_scaling', MinMaxScaler(), ['f1', 'f2'],
        'robust_scaling', 'RobustScaler(), ['f3', 'f4'],
        ],
        remainder = 'passthrough'
)
xtrain_new = preprocessing.fit_transform(xtrain)
* Here the xtrain will have 6 columns, because ot keeps the reamining caolumns


