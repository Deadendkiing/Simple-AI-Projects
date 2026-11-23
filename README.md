# Simple AI Projects

![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E?logo=huggingface&logoColor=black)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)

A collection of AI, machine learning and data analysis projects I built and presented during my Computer Science studies, now as a Masters student. They range from first steps with NumPy and pandas to deep learning, NLP and fine-tuning BERT.

Every notebook is saved with its outputs, so you can read the code, charts and results right here on GitHub without running anything.
Feel free to use anything here for your own projects or presentations.

## Highlights

| Project | Approach | Result |
|---|---|---|
| [MNIST digit classification](data-mining/mnist-classifiers-comparison.ipynb) | Random Forest vs KNN vs SVM, tuned with GridSearchCV, plus a Voting ensemble | **98.0%** test accuracy (SVM) |
| [Movie review sentiment with BERT](deep-learning-nlp/sentiment-bert-transformers.ipynb) | Fine-tuned `bert-base-uncased` with Hugging Face Transformers | **87.2%** accuracy, F1 0.87 |
| [Sentiment: LSTM vs VADER](deep-learning-nlp/sentiment-rnn-vs-vader.ipynb) | Recurrent neural network compared with a rule-based analyzer | LSTM **79%** (AUC 0.88) vs VADER 70% |
| [Loan risk prediction](machine-learning/loan-risk-imbalanced-learning.ipynb) | Balanced Random Forest and Easy Ensemble on 68k LendingClub loans | **0.87** balanced accuracy |
| [Credit card fraud detection](deep-learning-nlp/credit-card-fraud-detection.ipynb) | Neural network + SMOTE on 285k transactions (0.17% fraud) | **82%** of frauds caught |
| [Diabetes prediction](machine-learning/diabetes-classification-report.ipynb) | Logistic regression on the Pima Indians dataset | **78%** accuracy |

## All projects

### 🧠 [Deep Learning & NLP](deep-learning-nlp)
- **Sentiment analysis** of 25,000 IMDB reviews: an LSTM against VADER, and a fine-tuned BERT model
- **Gold price direction** with an LSTM and a logistic-regression baseline. Both land around 50%, a good reminder of how hard markets are to predict
- **Credit card fraud detection** on a highly imbalanced dataset
- **Neural network basics** with Keras on synthetic blobs and moons

### ⛏️ [Data Mining](data-mining) (Masters, term 2)
- **MNIST classifier comparison**: the term project
- **Pima diabetes**: exploratory analysis, logistic regression, and Euclidean / Manhattan / Minkowski distance metrics

### 📈 [Machine Learning](machine-learning)
- **Bank loan approval**: logistic regression vs SVM
- **Loan risk classification** with imbalanced-learn ensembles
- **Diabetes classification** with confusion matrix and classification report

### 📊 [Data Analysis](data-analysis)
- **Pandas**: cryptocurrency prices and BlackBerry stock returns
- **SQL**: loading CSV data into SQLite and querying it from Python

### 📝 [Course Exercises](course-exercises)
Seven step-by-step exercises: NumPy, reading and aggregating CSV files, pandas on people / customers / S&P 500 data, and an RNN assignment on gold prices.

### 🔧 [Misc](misc)
Weather from the OpenWeatherMap API, face detection with OpenCV, and a simple chatbot API client.

## Repository structure

```
Simple-AI-Projects/
├── data-mining/          # each folder has its own README
│   ├── *.ipynb
│   └── data/             # datasets used by the notebooks in this folder
├── deep-learning-nlp/
├── machine-learning/
├── data-analysis/
├── course-exercises/
├── misc/
└── requirements.txt
```

## Running the notebooks

```bash
git clone https://github.com/Deadendkiing/Simple-AI-Projects.git
cd Simple-AI-Projects
pip install -r requirements.txt
jupyter notebook
```

- Open each notebook **from inside its folder**. Notebooks load their data from the folder's `data/` directory.
- The three largest datasets are stored as `.zip` files. pandas reads them directly, so there's no need to unzip them.
- In **Google Colab**, upload the notebook together with its `data/` folder.
- The BERT notebook needs a GPU (Colab's free T4 is enough).

## Datasets

| Dataset | Used in |
|---|---|
| [MNIST](http://yann.lecun.com/exdb/mnist/) (downloaded automatically by Keras) | Data Mining |
| [Pima Indians Diabetes](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) | Data Mining, Machine Learning |
| IMDB movie reviews (25,000 labelled reviews) | Deep Learning & NLP |
| [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) | Deep Learning & NLP |
| LendingClub loans, Q1 2019 | Machine Learning |
| Gold, crypto and stock prices, S&P 500 companies, sample people / customer records | Data Analysis, Course Exercises |

All datasets are included in the repository.
