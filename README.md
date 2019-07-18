# kaggle_dont_call_me_turkey
Case study of Kaggle competition: Don't call me turkey

# Results
|           	| GRU + <br>Attention + FC 	| Bidirectional GRU + <br>Attention + FC 	| GRU + <br>GlobalAveragePooling1D + FC 	|
|-----------	|----------------------	|------------------------------------	|-----------------------------------	|
| Accracy   	| 1                    	| 1                                  	| 1                                 	|
| Log Loss  	| 0.0011               	| 2.87E-04                           	| 0.007                             	|
| AUC score 	| 1                    	| 1                                  	| 1                                 	|

# Key APIs
  - Decomposition
    - sklearn.decomposition.PCA(n_components)
- Data Manipulation
  - Fill NULL
    - pandas.DataFrame.fillna(-1)
    - pandas.DataFrame.isnull().any().any()
  - Convert List of List to a single List
    - lambda x: list(itertools.chain.from_iterable(x))
