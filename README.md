# binary_mushrooms_rf
kaggle competition for binary classification of poisonous mushrooms, using random_forest

# Mushrooms Binary Classification / Random Forest
In this notebook:  

* Using extra dataset
* Retaining all columns and encoding NaN values as a distinct category (for categorical features)
* Use a utility script to encoding by frequency, [here the script](https://www.kaggle.com/code/crisbebop/frequency-encoder-py)
* Imputing missing values (numerical features) using KNN
* Performing 5-fold cross-validation
* Saving OOB (Out-Of-Bag) predictions

## Previous results OOB

|Criterion | Estimators| Preprocess | OOB MCC|Cross-val Time spent (min)|
-----------|-----------|------------|--------|----------------|
| Gini | 100 | extra_data+Clean_noise+FE+KNN_imp+Robust|0.98449 |
| Gini | 300 | " | 0.98454 | |
| Gini | 500 | "  | 0.98455 |174.82|
| Entropy| 100 | " | 0.98448 | |
| Entropy| 300 | " |  0.98454| |
| Entropy | 500 |  " | 0.98457| 162.35 |
| Entropy | 500 | extra_data+FE+KNN_imp+Robust | 0.98460 | 141.77 |

