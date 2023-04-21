# FP-Growth-Algorithm
A more efficient way to find frequent itemsets in a large dataset compared to apriori algorithm.
Here are the functions in this model, please feel free to use them.

## set_param(sup = 10, con = 0.6):
Set `min_support` and `confidence` to specific value according to the argument. If no parameter is delivered, then the default value is 10 for  `min_support` and 0.6 for  `confidence`.

## show_param(*args):
Show all global variables in the module:
+ min_support: This variable indicates the minimum support value when creating FP Tree. The default value is 10.

## FP_Growth_Min(df):
The main function in this module. To conduct the FP-Growth algorithm, you need to put a `pandas.Dataframe` object as an argument.</br>
The function will return a `pandas.Dataframe` object with columns: ['frequent itemset',  'support', 'antecedent', 'consequent', 'confidence', 'lift'].
