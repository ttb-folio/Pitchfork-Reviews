# Pitchfork Music Reviews
Exploring Pitchfork Reviews kaggle dataset

Dataset: https://www.kaggle.com/nolanbconaway/pitchfork-data

Binary Classification of Pitchfork Reviews by conducting sentiment analysis on review text.
Reviews Score (0-10 scale) is transformed into two classes by thresholding on the median score.

Data Loading and EDA -> Takes sqlite database from kaggle and creates csv files into Data Folder. Some plots (Seaborn)

Baseline Sentiment Analysis -> Random Model and Logistic Regression (sklearn)

Sentiment Analysis Classifier GPU -> DistilBERT model (HuggingFace)

Sentiment Analysis TPU -> Code modified to run on TPU using PyTorch XLA.

To view pandas-profiling reports in ProfileReports folder, use: https://htmlpreview.github.io

Next Steps: Model peforms perfect binary classification. Can it learn to predict on a finer granularity? Increase number of classes. Possibly condition on genre or review author.
