# 🎓 Jamboree Education Linear Regression Project

This project uses the **Jamboree Education dataset** to predict graduate school admission chances based on academic scores and personal profile features. 
The primary goal is to explore relationships between variables and build accurate linear regression models.

---

## 📁 Project Structure

```
🔹 Jamboree_LinearRegression.ipynb     # Main Jupyter Notebook for analysis and modeling
🔹 data/
🔹🔹 Jamboree_Admission.csv          # Dataset file
🔹 models/                             # Saved regression models
🔹 visualizations/                     # Generated plots and visualizations
🔹 README.md                           # Project overview and documentation
```

---

## 📊 Dataset Description

The dataset contains the following variables:

| Feature             | Description                                   |
| ------------------- | --------------------------------------------- |
| `GRE Score`         | Graduate Record Examination score             |
| `TOEFL Score`       | Test of English as a Foreign Language score   |
| `University Rating` | University quality rating (1 to 5)            |
| `SOP`               | Strength of Statement of Purpose (1 to 5)     |
| `LOR`               | Strength of Letter of Recommendation (1 to 5) |
| `CGPA`              | Undergraduate GPA (out of 10)                 |
| `Research`          | Research experience (0 = No, 1 = Yes)         |
| `Chance of Admit`   | Probability of admission (0.0 to 1.0)         |

---

## 💠 Key Steps

### 🔹 Data Preprocessing

* Loaded dataset and removed duplicates and outliers
* Checked for and handled missing values

### 🔹 Exploratory Data Analysis (EDA)

* Plotted distributions and boxplots for feature insights
* Generated a correlation heatmap to evaluate feature relationships

### 🔹 Modeling

* Built an **Ordinary Least Squares (OLS)** linear regression model
* Evaluated using:

  * R-squared (R²)
  * Mean Absolute Error (MAE)
  * Root Mean Squared Error (RMSE)
* Compared performance of:

  * **Ridge Regression**
  * **Lasso Regression**
  * **ElasticNet Regression**

---

## 📈 Linear Regression Workflow

The modeling and evaluation include:

* ✔️ **EDA**: Histograms, boxplots, scatterplots
* ✔️ **Correlation Analysis**
* ✔️ **Model Building**: Linear, Ridge, Lasso, ElasticNet
* ✔️ **Assumption Testing**: Multicollinearity, homoscedasticity, normality
* ✔️ **Model Evaluation**: MAE, RMSE, R², Adjusted R²

---

## 💡 Key Insights

* **CGPA** is the strongest predictor of admission.
* **GRE** and **TOEFL** scores positively impact admission chances.
* **Research experience** significantly improves admission probability.
* **SOP** and **University Rating** have weaker influence compared to academic scores.

---

## 📦 Installation & Requirements

To run this project locally or in Google Colab, install the following libraries:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
```

---

## 🚀 How to Run

1. Clone the repository.
2. Open `Jamboree_LinearRegression.ipynb` in **Jupyter Notebook** or **Google Colab**.
3. Ensure `Jamboree_Admission.csv` is inside the `/data` folder.
4. Run all cells to explore EDA and model training.

---

## 📊 Results

* The OLS model achieved **R² = 0.826**, explaining **82.6%** of the variance in admission chances.
* The model confirms that **academic performance** and **research experience** are key drivers for admission.

---

## 🔭 Future Improvements

* Add additional features such as internships, GPA trend, or publication count.
* Explore non-linear models (e.g., Decision Trees, XGBoost) for better accuracy.
* Implement a simple web app using Flask/Streamlit for interactive predictions.

---

## 📄 License

This project is licensed under the MIT License.
.
