Phishing Website Detection with Machine Learning
Overview
This project applies machine learning techniques to classify websites as either phishing or legitimate using a structured phishing website dataset. The project investigates how well different machine learning models perform on this cybersecurity task and analyzes which categories of features contribute most to predictive performance.

Research Question
Can phishing websites be accurately detected using machine learning, and which feature groups are most useful for detection?

Dataset
This project uses the Web page Phishing Detection Dataset from Kaggle:

Web page Phishing Detection Dataset

The dataset contains 11,430 samples and 89 columns, including a binary target label (status) indicating whether a website is phishing or legitimate.

Project Structure
phishing-website-detection-ml/
├── data/
│   └── raw/
│       └── dataset_phishing.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_model_baselines.ipynb
│   ├── 04_model_comparison.ipynb
│   └── 05_ablation_study.ipynb
├── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│   └── utils.py
├── requirements.txt
├── README.md
└── finalreport.pdf
Notebooks
01_data_cleaning.ipynb: Loads, cleans, and prepares the dataset for modeling
02_eda.ipynb: Performs exploratory data analysis and feature investigation
03_model_baselines.ipynb: Trains baseline models including Logistic Regression and Decision Tree
04_model_comparison.ipynb: Compares stronger models including Random Forest and Gradient Boosting
05_ablation_study.ipynb: Evaluates the predictive power of different feature groups
Models Used
Logistic Regression
Decision Tree
Random Forest
Gradient Boosting
Main Results
The best-performing model was Random Forest, with the following test performance:

Accuracy: 0.9602
Precision: 0.9566
Recall: 0.9641
F1 Score: 0.9603
ROC-AUC: 0.9935
The ablation study showed that:

using all features together produced the best results
domain/trust features were the strongest individual feature group
URL/lexical and hyperlink/page-based features also contributed meaningful predictive power
Key Findings
Phishing websites can be detected effectively using classical machine learning methods
Ensemble methods outperformed simpler baseline models
Domain reputation and trust-related features were especially important for classification
Combining multiple feature groups led to the strongest overall performance
How to Run
Clone the repository
Install the required packages with pip install -r requirements.txt
Open the notebooks in VS Code or Jupyter
Run the notebooks in order from 01_data_cleaning.ipynb through 05_ablation_study.ipynb
Final Report
The final written report for this project is included as finalreport.pdf

I removed the fenced code block version and used an indented block instead, so it won’t break on you.

After you paste and save it, if you want, I can help you with the next exact step:

commit the README
push it
then start the final report outline




