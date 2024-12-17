## **hw4-1**

1. **Business Understanding**:  
   Compare 16 machine learning models to predict survival (`Survived`) on the Titanic dataset.

2. **Data Understanding**:  
   Use a multi-feature dataset while removing irrelevant columns (`Name`, `Ticket`, `Cabin`).

3. **Data Preparation**:  
   Automatically handle preprocessing (e.g., missing values, scaling) using PyCaret.

4. **Modeling**:  
   Train and compare 16 models to rank their performance.

5. **Evaluation**:  
   Visualize model performance using AUC curves and confusion matrices.

6. **Deployment**:  
   Prepare results for saving or further use.

   # Model Optimization using PyCaret and Optuna



## **hw4-2**

### 1. **Feature Engineering**
   - Load the Titanic dataset and drop irrelevant columns (`Name`, `Ticket`, `Cabin`).
   - Create two new engineered features:
     - `Family_Size`: Combines `SibSp` and `Parch`.
     - `Fare_Per_Person`: Adjusts `Fare` by family size.

### 2. **Model Selection**
   - Use PyCaret for automated classification setup.
   - Use Optuna to optimize hyperparameters for selected models:
     - **Random Forest (rf)**
     - **XGBoost (xgboost)**
     - **LightGBM (lightgbm)**
     - **Extra Trees (et)**.

### 3. **Training and Hyperparameter Optimization**
   - Run 30 Optuna trials to tune the hyperparameters for each model.
   - Optimize based on **Accuracy**.

### 4. **Evaluation**
   - Plot the AUC curve and confusion matrix for the best-optimized model.

### 5. **Save the Optimized Model**
   - Save the final model for future predictions using `save_model`.

---

## **Tools Used**
- **PyCaret**: Simplifies model training and evaluation.
- **Optuna**: Automates hyperparameter tuning for optimal performance.

---

### **Goal**
Optimize and compare models to achieve the best classification accuracy.


