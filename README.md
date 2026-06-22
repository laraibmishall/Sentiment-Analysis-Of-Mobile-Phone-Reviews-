Readme sentiment analysis · MDCopy📱 Mobile Review Sentiment Analysis



A machine learning project that classifies smartphone customer reviews into Positive, Negative, and Neutral sentiments using three models — Logistic Regression, Random Forest, and CNN — with an interactive Streamlit dashboard for visualization.


📌 Project Overview

This project analyzes real-world customer reviews for 5 popular smartphones scraped from online platforms. It preprocesses the raw text, trains multiple ML/DL classifiers, compares their performance, and presents results through a fully interactive web dashboard.


📦 Dataset

DetailInfoPhones Covered5 devicesRaw Reviews50,500After Cleaning10,769Sentiment ClassesPositive · Negative · NeutralTrain / Test Split80% / 20%

Phones Analyzed:


Samsung Galaxy S24 Ultra
Apple iPhone 15 Pro
Google Pixel 8 Pro
OnePlus 12
Xiaomi Redmi Note 13 Pro



🤖 Models & Performance

ModelAccuracyPrecisionRecallF1 ScoreLogistic Regression98.28%99.21%98.28%98.61%Random Forest99.12%99.18%99.12%99.14%CNN ✅99.30%99.49%99.30%99.36%


✅ CNN achieved the best overall performance across all metrics.




📁 Project Structure

sentiment-analysis/
│
├── data/
│   ├── apple_iphone_15_pro_reviews.txt
│   ├── google_pixel_8_pro_reviews.txt
│   ├── oneplus_12_reviews.txt
│   ├── samsung_galaxy_s24_ultra_reviews.txt
│   └── xiaomi_redmi_note_13_pro_reviews.txt
│
├── output/
│   └── phone_sentiment.xlsx         # Sentiment predictions output
│
├── ids_project.ipynb                # Full ML pipeline (EDA, training, evaluation)
├── sentiment_dashboard.py           # Streamlit interactive dashboard
├── mobile_reviews_cleaned.xlsx      # Cleaned dataset
└── PROJECT REPORT.docx              # Full project report


📊 Dashboard Features

The Streamlit dashboard includes:


Live Sentiment Predictor — Enter any review text and get instant sentiment classification with class probabilities
Model Comparison — Side-by-side accuracy, precision, recall, and F1 scores for all 3 models
Confusion Matrices — Per-model confusion matrix visualization
CNN Training History — Accuracy and loss curves over 10 epochs
Dataset Statistics — Review counts and sentiment distribution per phone
Sample Reviews — Real labelled review examples for each device



🚀 How to Run

1. Install Dependencies

bashpip install streamlit pandas numpy matplotlib seaborn scikit-learn tensorflow openpyxl

2. Run the Dashboard

bashstreamlit run "sentiment_dashboard.py"

3. Open Jupyter Notebook (for full pipeline)

bashjupyter notebook ids_project.ipynb


🛠️ Tech Stack

ToolPurposePythonCore languageScikit-learnLogistic Regression & Random ForestTensorFlow / KerasCNN modelStreamlitInteractive dashboardPandas & NumPyData processingMatplotlib & SeabornVisualizationsOpenPyXLExcel output
