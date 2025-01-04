# Important Notes:
- Better to be launched via Google CoLab.
- If launched through Google CoLab, upload the `.xlsx` file first.
- If launched through Jupyter Notebook, double check the path when reading the file via read_excel('path').
- First launch through Google CoLab will require you to Restart the session to implement `pip` installation for the PyCaret libraries. So, please conform to the process and press on `Restart Session`, and run the cells again.
# Project Description and Notes:
### **Algorithm Selection**:
I chose Light Gradient Boosting Machine (LightGBM) for several reasons:
- It handles both numerical and categorical features well.
- Excellent performance with tabular data.
- Good handling of non-linear relationships.
- Fast training speed.
- Built-in handling of missing values.
- Good performance with numerical target variables.
### **Feature Selection**:
- Used all available features (Age, Dur) as they all likely influence PPV.
- Gender as categorical feature.
- Age and Dur (Duration) as numerical features.
### **Evaluation Strategy**:
- Implemented 5-fold cross-validation for robust performance assessment.
- Used multiple evaluation metrics:
	- RMSE (Root Mean Squared Error) as primary metric.
	- MAE (Mean Absolute Error) as secondary metric.
	- R² score for overall fit assessment.
### **Model Tuning**:
- Included automated hyperparameter tuning using grid search.
- Optimized for RMSE to minimize prediction errors.
### **Additional Features**:
- Feature importance analysis to understand predictor significance.
- Cross-validation prediction for robust performance estimation.
- GPU support if available for faster training.
