# CodeClause_Market-Basket-Analysis-in-Python-using-Apriori-Algorithm
# Description 
Whenever you visit a retail supermarket, you will find that baby diapers and wipes, bread and butter, pizza base and cheese, beer, and chips are positioned together in the store for sales. This is what market basket analysis is all about analyzing the association among products bought - together by customers. Market basket analysis is a versatile use case in the retail industry that helps cross-sell products in a physical outlet and also helps e-commerce businesses recommend products to customers based on product associations. Apriori and FP growth are the most popular machine learning algorithms used for association learning to perform market basket analysis.
## Import Packages
```
import numpy as np
import pandas as pd
from apyori import apriori
from collections import Counter
```
## Convert df to list
```
df.values.tolist()
```
## Remove 'Nan' values
```
T = []
for i in range(len(df)):
    T.append([str(df.values[i,j]) for j in range(0, 20)if str(df.values[i,j])!='nan'])
```
## Set Rules for Apriori model
```
rules = apriori(T, min_support= 0.003,min_confidence=0.35,min_lift=3,min_length=2)
```
## Result
```
list(rules)
```
[RelationRecord(items=frozenset({'escalope', 'pasta'}), support=0.005865884548726837, ordered_statistics=[OrderedStatistic(items_base=frozenset({'pasta'}), items_add=frozenset({'escalope'}), confidence=0.3728813559322034, lift=4.700811850163794)]) \
This means the person who baught 'escalope', 'pasta' has 37% more likely to buy 'pasta'.\
We can change min_confidence according our need.
