# Customer Retails Dataset — Various ML Models and compare them

A supervised machine learning project that builds and compares multiple classification models on a customer retail dataset. The project covers the complete ML workflow — from preprocessing and visualization to model training, evaluation, and comparison.

## Project Objective

To implement various Machine Learning models on a customer retail dataset and compare their performance, gaining hands-on experience with preprocessing, visualization, model training, prediction, evaluation, and algorithm comparison.

## Overview

| Item | Detail |
|---|---|
| **Dataset** | Customer retail transactions (`customer_retail.csv.xlsx`) |
| **Task** | Multi-class classification — predict `Country` from purchase features |
| **Features used** | `Quantity`, `UnitPrice`, `Country` |
| **Target** | `Country` (label-encoded) |
| **Models** | Logistic Regression, Decision Tree, K-Nearest Neighbours |
| **Evaluation** | Accuracy Score, Confusion Matrix |

## Project Structure

```
├── Customer_retails_Datasets_Build_ML_Model.ipynb
├── customer_retail.csv.xlsx
└── README.md
```

## Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib scikit-learn openpyxl
```

### Running the Notebook

1. Clone this repository
   ```bash
   gh repo clone dhanasekaran65/Customer_Detail_Dataset_Build_Various_ML-Model
   cd Customer_Detail_Dataset_Build_Various_ML-Model
   ```
2. Place `customer_retail.csv.xlsx` in the project root.
3. Launch Jupyter and open the notebook
   ```bash
   jupyter notebook Customer_retails_Datasets_Build_ML_Model.ipynb
      ```

> **Google Colab users:** The notebook expects the dataset at `/content/customer_retail.csv.xlsx`. Upload the file to your Colab session before running.

## Project Workflow

1. **Load dataset** — read customer retail data using Pandas
2. **Handle missing values** — drop rows with null entries
3. **Encode categorical columns** — convert `Country` to integers using `LabelEncoder`
4. **Visualize data** — scatter plot of Quantity vs UnitPrice (Customer Distribution Graph)
5. **Split data** — 80/20 train/test split with `random_state=42`
6. **Train Logistic Regression** — fit and predict
7. **Train Decision Tree** — fit and predict
8. **Train KNN** — fit and predict
9. **Evaluate models** — accuracy score and confusion matrix for each
10. **Compare performance** — bar chart of all model accuracies

## Models & Evaluation

Each model is trained and evaluated on the same dataset split.

| Model | Accuracy | Confusion Matrix |
|---|---|---|
| Logistic Regression | ✓ | ✓ |
| Decision Tree Classifier | ✓ | ✓ |
| K-Nearest Neighbors (KNN) | ✓ | ✓ |

A final **Model Accuracy Comparison Graph** visualises all three results together.

## Visualizations

- **Customer Distribution Graph** — scatter plot of Quantity vs UnitPrice
- **Model Accuracy Comparison Graph** — bar chart comparing all three classifiers
  
## Libraries Used

- [pandas](https://pandas.pydata.org/) — data loading and manipulation
- [NumPy](https://numpy.org/) — numerical operations
- [Matplotlib](https://matplotlib.org/) — data visualisation
- [scikit-learn](https://scikit-learn.org/) — ML models, encoding, and evaluation

## Learning Outcomes

- Understand the complete Machine Learning workflow
- Understand supervised learning concepts
- Learn model evaluation techniques (accuracy, confusion matrix)
- Compare different ML algorithms on the same dataset
- Interpret graphs and confusion matrices

## Conclusion

This project demonstrates how different Machine Learning algorithms perform on the same dataset. It highlights the importance of preprocessing, feature selection, evaluation, and model comparison in real-world ML applications.
