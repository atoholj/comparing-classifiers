# Comparing Classifiers – Practical Application 17.1

This project compares four supervised machine learning classification algorithms using the **UCI Bank Marketing dataset**. The goal is to determine which model best predicts whether a customer will subscribe to a long-term deposit product during a telephone marketing campaign.

##  Business Objective
A Portuguese bank conducted multiple direct marketing campaigns aimed at increasing subscriptions to a term deposit investment product. Each row in the dataset represents a phone call to a client. The objective of this project is to build and evaluate several machine learning models to:

- Identify clients most likely to subscribe
- Improve campaign effectiveness
- Reduce unnecessary calls and associated costs

##  Dataset
The dataset originates from the **UC Irvine Machine Learning Repository** and includes:

- **Client attributes** such as age, job, marital status, education, and existing loans  
- **Campaign-related features** including contact method, month, day of week, call duration, and previous outcomes  
- **Macroeconomic indicators** such as euribor rate, consumer confidence, and employment variation  
- **Target variable:** `y` — whether the client subscribed to the term deposit (“yes” or “no”)

Files included in this repository:

- `bank-additional-full.csv`  
- `bank-additional.csv`  
- `bank-additional-names.txt`  

##  Data Preparation
The notebook includes:

- Handling categorical variables with one-hot encoding  
- Train/test splitting of the dataset  
- Scaling numerical variables for appropriate algorithms  
- Optional removal of the `duration` feature (since it is only known after a call is completed)  
- Basic data exploration and summary statistics  

##  Models Implemented
Four classification algorithms were built and evaluated:

1. **k-Nearest Neighbors (KNN)**
2. **Logistic Regression**
3. **Decision Tree Classifier**
4. **Support Vector Machine (SVM)**

These models were selected to compare linear, non-linear, distance-based, and tree-based approaches.

##  Evaluation Metrics
Each model was compared using:

- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1 Score**  
- **Confusion Matrix**

These metrics provide a comprehensive view of overall performance and the ability to identify true positive subscription outcomes.

##  Findings & Insights
A detailed comparison of all models is included in the Jupyter Notebook. Key insights include:

- Performance differences across models  
- Trade-offs between interpretability and predictive power  
- Which classifier is most effective for the bank’s marketing objective  
- Recommendations for next steps such as tuning, feature engineering, or ensemble methods  

##  Repository Structure
```text
comparing-classifiers/
│
├── comparing_classifiers.ipynb      # Main assignment notebook
├── README.md                        # Project overview
│
└── data/
    └── bank-additional/
        ├── bank-additional-full.csv
        ├── bank-additional.csv
        └── bank-additional-names.txt
