# Simple-AI-Projects
Some simple AI projects for college

Hi,
I'm a Masters computer Science student and this Repository Contains Small Projects That i Presented for college.
Feel Free to use everything for your projects or presentations too.

## Projects

| Folder | What's inside |
|---|---|
| [`data-mining/`](data-mining) | Masters term 2 data-mining coursework: MNIST classifier comparison (Random Forest, KNN, SVM, Voting), Pima diabetes EDA, logistic regression, distance metrics |
| [`deep-learning-nlp/`](deep-learning-nlp) | Sentiment analysis (LSTM vs VADER, BERT), gold price prediction with an RNN, credit-card fraud detection, TensorFlow basics |
| [`machine-learning/`](machine-learning) | Bank loan approval, LendingClub loan-risk with imbalanced learning, diabetes classification |
| [`data-analysis/`](data-analysis) | Pandas analysis of crypto and stock prices, loading data into SQLite |
| [`course-exercises/`](course-exercises) | Step-by-step exercises: NumPy, CSV handling, Pandas, and an RNN assignment |
| [`misc/`](misc) | Weather API, face detection with OpenCV, a simple chatbot API client |

## Running the notebooks

Every notebook was written in Google Colab and saved with its outputs, so you can read the results directly on GitHub.

To run one yourself:

```bash
pip install -r requirements.txt
```

Then open the notebook **from inside its folder** — each folder has a `data/` subfolder and the notebooks load files from there (e.g. `data/diabetes.csv`).
The three largest datasets are stored as `.zip` files; pandas reads them directly, so there is no need to unzip them.

In Colab, upload the notebook together with its `data/` folder.
