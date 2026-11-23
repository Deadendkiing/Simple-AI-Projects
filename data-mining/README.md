# Data Mining (Masters, Term 2)

| Notebook | Description |
|---|---|
| [`mnist-classifiers-comparison.ipynb`](mnist-classifiers-comparison.ipynb) | **Term project** (پروژه داده کاوی). Classifies MNIST handwritten digits with Random Forest, KNN and SVM, tunes each with `GridSearchCV`, combines them in a Voting classifier and compares accuracies (~97–98% on the test set). |
| [`diabetes-eda.ipynb`](diabetes-eda.ipynb) | Exploratory data analysis of the Pima Indians Diabetes dataset with pandas and seaborn plots. |
| [`diabetes-logistic-regression.ipynb`](diabetes-logistic-regression.ipynb) | Prediction model based on logistic regression (مدل پیش بینی بر اساس Logistic regression): missing-value handling, scaling, accuracy and confusion matrix. |
| [`distance-metrics.ipynb`](distance-metrics.ipynb) | Computing Euclidean, Manhattan and Minkowski distances between records of the dataset (محاسبه فواصل اقلیدوسی، منهتن، مینکوفسکی). |
| [`math-and-sigmoid-basics.ipynb`](math-and-sigmoid-basics.ipynb) | Small class exercise: `exp`, `log` and a sigmoid function. |

## Data
- `data/pima-indians-diabetes.data.csv` — [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) (768 rows).
- MNIST is downloaded automatically by `tensorflow.keras.datasets`.
