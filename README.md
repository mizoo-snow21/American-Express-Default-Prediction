# American-Express-Default-Prediction

https://www.kaggle.com/competitions/amex-default-prediction/leaderboard
We got 221th prize.  
This is summary and codes.

# Summary

## Data strategy
・5fold StratifiedKFold  
・Deferent features using Null importance and Permutation importance  
https://www.kaggle.com/code/ogrellier/feature-selection-with-null-importances  
https://scikit-learn.org/stable/modules/permutation_importance.html  

# Model
## microsoft/deberta-v3-large
・TransformerHead + multisampledropout  
・optimizer = AdamW  
・epoch = 5  
・scheduler = CosineAnnealingLR  

## anferico/bert-for-patents
・TransformerHead  
・optimizer = AdamW   
・epoch = 5    
・scheduler = CosineAnnealingLR  

## Weight optimazation 
I use weight optimazation to maximize cv.  
 cv = 0.7994    
 lb = 0.80735

