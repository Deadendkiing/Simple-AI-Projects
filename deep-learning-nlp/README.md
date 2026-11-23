# Deep Learning & NLP

| Notebook | Description |
|---|---|
| [`sentiment-rnn-vs-vader.ipynb`](sentiment-rnn-vs-vader.ipynb) | Sentiment analysis of movie reviews: an LSTM recurrent neural network compared with NLTK's rule-based VADER, using confusion matrices and classification reports. |
| [`sentiment-bert-transformers.ipynb`](sentiment-bert-transformers.ipynb) | Fine-tuning `bert-base-uncased` (Hugging Face Transformers + PyTorch) on the same movie reviews. A GPU is recommended. |
| [`gold-price-rnn.ipynb`](gold-price-rnn.ipynb) | Predicting whether the gold price goes up or down with an LSTM network on 60-day windows. |
| [`gold-price-logistic-regression.ipynb`](gold-price-logistic-regression.ipynb) | Baseline: logistic regression on the previous close plus a (synthetic) sentiment feature, evaluated with ROC/AUC. |
| [`credit-card-fraud-detection.ipynb`](credit-card-fraud-detection.ipynb) | Neural network for fraud detection on a highly imbalanced dataset, using SMOTE oversampling. |
| [`tensorflow-neural-network-basics.ipynb`](tensorflow-neural-network-basics.ipynb) | Introduction to Keras neural networks on `make_blobs` and `make_moons` data. |

## Data
| File | Contents |
|---|---|
| `data/movie_comments.zip` | 25,000 IMDB movie reviews (`comment`, `sentiment`). |
| `data/gold_cad.csv` | Daily gold close price in CAD, 2001 onwards. |
| `data/transactions.zip` | 284,807 card transactions — the [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) dataset. |

The `.zip` files are read directly with `pd.read_csv`, no unzipping needed.
