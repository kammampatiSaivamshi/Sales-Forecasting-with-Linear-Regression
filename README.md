#  Sales Forecasting Using Machine Learning

This project demonstrates a full-cycle machine learning pipeline for **Sales Forecasting**, including data preprocessing, feature engineering, model training, and evaluation. It is designed as part of a real-time internship with a structured step-by-step approach.

---

##  Project Structure

1. **Data Loading & Exploration**

   * Importing libraries
   * Loading the dataset (`train.csv`)
   * Initial exploration (`head()`, `info()`, `describe()`)

2. **Data Cleaning & Preprocessing**

   * Handling missing values
   * Converting date formats
   * Encoding categorical features

3. **Feature Engineering**

   * Extracting useful date parts (month, year, etc.)
   * Creating new features to enhance model performance

4. **Modeling & Forecasting**

   * Splitting data into training and testing sets
   * Using machine learning models (e.g., Linear Regression, Random Forest, XGBoost)
   * Evaluating models using RMSE, MAE, and R² Score

5. **Conclusion**

   * Best model selected based on performance
   * Insights for improving sales strategy

---

##  Technologies Used

* Python 🐍
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn (for visualization)
* Jupyter Notebook

---

##  Dataset

The dataset used in this project contains:

* Date
* Store ID
* Product Category
* Units Sold
* Revenue

*(Dataset path used in notebook: `train.csv`)*

---

##  How to Run

1. Clone the repository or download the `.ipynb` notebook.
2. Make sure you have Python and Jupyter Notebook installed.
3. Install required libraries:

   ```bash
   pip install pandas scikit-learn matplotlib seaborn xgboost
   ```
4. Run the notebook:

   ```bash
   jupyter notebook Sales_Forecasting.ipynb
   ```

---

##  Future Enhancements

* Add time-series based models (e.g., ARIMA, Prophet)
* Automate hyperparameter tuning
* Build a Streamlit dashboard for real-time sales forecasting

---

## Contributing

Feel free to contribute to this project by submitting bug reports, features, or enhancements through issues or pull requests.

### 🙋‍♂️ Author

**Kammampati Saivamshi**
*Aspiring Data Scientist*
📫 Reach me on [LinkedIn](https://www.linkedin.com)


