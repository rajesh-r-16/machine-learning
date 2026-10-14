# Machine Learning Algorithm Comparison

A machine learning project demonstrating **Boosting, Clustering, and Classification** using Python, Scikit-learn, XGBoost, Pandas, NumPy, and Matplotlib. The project compares multiple algorithms on three datasets, evaluates their performance, and identifies the best-performing model using suitable evaluation metrics.

## 📌 Project Overview

This repository contains three machine learning experiments:

1. **Boosting — Medical Insurance Cost Prediction**
2. **Clustering — Mall Customer Segmentation**
3. **Classification — Social Network Ads Purchase Prediction**

Each experiment includes dataset preparation, model training, testing, evaluation, and algorithm comparison.

## 🎯 Objectives

- Understand and implement different machine learning algorithms.
- Train and test multiple models using separate datasets.
- Evaluate model performance using appropriate metrics.
- Compare algorithms and identify the best-performing model.
- Visualize results for easier interpretation.
- Practice machine learning implementation using Google Colab and Python.

## 🗂️ Repository Structure

```text
machine-learning/
│
├── Data/
│   ├── insurance_pre.csv
│   ├── Mall_Customers.csv
│   └── Social_Network_Ads.csv
│
├── Notebook/
│   ├── Boosting.ipynb
│   ├── Clustering.ipynb
│   └── Classification.ipynb
│
├── PDF/
│   └── Project documentation and reports
│
├── requirements.txt
└── README.md
```

*Note: The filenames above are examples of the intended organization. Use the actual filenames present in the repository.*

## 1. 🚀 Boosting — Medical Insurance Cost Prediction

**Dataset:** Medical insurance dataset (`insurance_pre.csv`)

**Objective:** Predict medical insurance charges based on customer information.

### Features

- Age
- Sex
- Body Mass Index (BMI)
- Number of children
- Smoking status

**Target variable:** `charges`

### Algorithms Used

| Algorithm | Description |
|---|---|
| AdaBoost Regressor | Combines weak learners to improve prediction performance. |
| Gradient Boosting Regressor | Builds sequential trees that correct previous prediction errors. |
| XGBoost Regressor | Uses optimized gradient boosting with regularization. |

### Evaluation Metrics

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

**Best model:** Determined by comparing the test-set R² score and prediction errors. Higher R² and lower MAE/RMSE are generally preferred.

## 2. 📊 Clustering — Mall Customer Segmentation

**Dataset:** Mall Customers (`Mall_Customers.csv`)

**Objective:** Group customers according to their annual income and spending behavior.

### Features

- Annual Income
- Spending Score

### Algorithms Used

| Algorithm | Description |
|---|---|
| K-Means | Groups customers around cluster centroids. |
| Agglomerative Clustering | Creates hierarchical groups based on similarity. |
| DBSCAN | Identifies dense customer groups and detects noise points. |

### Evaluation Metrics

- Silhouette Score
- Davies–Bouldin Index
- Calinski–Harabasz Score

**Best model:** Evaluated primarily using the Silhouette Score, with other cluster metrics and DBSCAN's noise percentage considered.

Clustering is an unsupervised learning task, so standard classification accuracy is not applicable without known ground-truth labels.

## 3. 🤖 Classification — Social Network Ads

**Dataset:** Social Network Ads (`Social_Network_Ads.csv`)

**Objective:** Predict whether a customer will purchase a product based on demographic and salary information.

### Features

- Gender
- Age
- Estimated Salary

**Target variable:** `Purchased`

- `0` — Not purchased
- `1` — Purchased

### Algorithms Used

| Algorithm | Description |
|---|---|
| Logistic Regression | Predicts purchase probability using a classification model. |
| Decision Tree | Predicts purchase outcomes using decision rules. |
| Random Forest | Combines multiple decision trees to make predictions. |

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

**Best model:** Determined by comparing test accuracy and reviewing precision, recall, and F1 score.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Development Environment:** Google Colab, Jupyter Notebook
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, XGBoost
- **Data Visualization:** Matplotlib
- **Version Control:** Git and GitHub

## ⚙️ Installation and Setup

### Option 1: Run in Google Colab

1. Open the notebook folder in this repository.
2. Select the notebook you want to execute.
3. Open it in Google Colab.
4. Upload the corresponding CSV dataset if required.
5. Run the cells sequentially.
6. Review the model scores, comparison tables, and charts.

### Option 2: Run Locally

Clone the repository:

```bash
git clone https://github.com/rajesh-r-16/machine-learning.git
```

Navigate to the project directory:

```bash
cd machine-learning
```

Install the required packages:

```bash
python -m pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the required notebook and execute its cells.

## 📈 Model Comparison and Results

Each notebook generates evaluation scores for its respective algorithms and identifies a leading model based on the selected metric.

| Experiment | Primary comparison metric | Preferred result |
|---|---|---|
| Boosting | R² Score | Higher |
| Clustering | Silhouette Score | Higher |
| Classification | Accuracy | Higher |

The final results depend on the dataset, train-test split, preprocessing, and model parameters. Actual scores should be generated by running the notebooks rather than assumed in advance.

## 💡 Applications

- Medical insurance cost estimation
- Customer segmentation and targeted marketing
- Purchase behavior prediction
- Machine learning algorithm evaluation
- Data-driven decision support

## 🔮 Future Enhancements

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
- Cross-validation for more reliable evaluation
- Additional machine learning algorithms
- Interactive dashboards for model results
- Model saving and deployment using Flask or FastAPI
- Improved visualizations and automated reports

## 👨‍💻 Author

**Rajesh R.**

GitHub: [@rajesh-r-16](https://github.com/rajesh-r-16)

## 📄 License

This project is intended for educational and learning purposes. Add an appropriate open-source license if you want others to reuse and redistribute the code.

---

⭐ If you find this project useful, consider starring the repository.

**Topics:** `machine-learning` · `python` · `scikit-learn` · `boosting` · `clustering` · `classification` · `xgboost` · `google-colab`
