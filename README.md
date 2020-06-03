# Home-Default-Credit-Risk

The Dataset is open-source from Kaggle https://www.kaggle.com/c/home-credit-default-risk/data

This dataset have many dimensions, many observations, and lots of missing values.

Missing values are imputed in R using missRanger package for variables have less than 60% of missing. Variables have more than 60% of missing are removed.

Nearly Zero Variance, VarImp, T-SNE are not useful for this dataset. Correlation is the only technique for PreProcessing.

Tuned Paramters of Random Forest, AdaBoost, Bagging DT, Xgboost, and then Tuning Stack Model are trained.
The submission score is ~76 based on AUC-ROC of Test Set.

This scored can be improved with Feature Engineering by creating new variables using existing variables to increase prediction power.

One-Class Classification is also performed. However, this is not suitable for AUC-ROC score because it does not give probabilistic output.


