# 🏠 House Prices Prediction

This project was developed as part of the [Kaggle competition: House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques). The objective is to predict house sale prices using machine learning techniques based on various property features.

---

## 📈 Competition Summary

- **Kaggle Score**: `0.13318`
- **Estimated Accuracy**: ~**86.68%**
- **Submission Type**: Regression (Root Mean Squared Log Error)

---

## 📁 Project Structure

- `House Prices Model.ipynb` – Main Jupyter Notebook with all code: data cleaning, preprocessing, feature engineering, model building, evaluation, and prediction.
- `final_predictions.csv` – The final output submitted to Kaggle.
- `.txt` files – Contain modular transformation or preprocessing functions used in the notebook.
- `README.md` – Project documentation (this file).

---

## 📊 Models Trained

Three machine learning models were trained and compared:

| Model                      | R² Score |
|---------------------------|----------|
| Decision Tree Regressor   | 0.7088   |
| Gradient Boosting Regressor | 0.9140 |
| **XGBoost Regressor (Final Model)** | **0.9192** |

The **XGBoost Regressor** was selected for final predictions due to its superior performance.

---

## ⚙️ Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

## 🧠 Key Steps

- **Data Cleaning**: Filled missing values using logic based on feature context.
- **Feature Engineering**:
  - Created binary and conditional features (e.g., `HasGarage`)
  - Addressed skewness and categorical inconsistencies
- **Encoding**: Dummification with alphabetically ordered binary columns
- **Normalization**: Min-Max scaling applied only to training numerical features
- **Model Selection**:
  - Hyperparameter tuning via `GridSearchCV` and `RandomizedSearchCV`
  - Final model trained on full training dataset

---

## 📌 Notes

- The notebook avoids log-transforming the target to preserve original interpretation.
- Evaluation was based on `R²` score locally, and **Root Mean Squared Log Error (RMSLE)** on Kaggle.
- The entire process was performed in Jupyter Notebook on macOS.

---

## 📜 License

This project is licensed under the **MIT License**. You're welcome to use, modify, and redistribute the code.

---

## 🙋‍♂️ Author

**Cihat Gecer**  
GitHub: [@cihatgecer](https://github.com/cihatgecer)
