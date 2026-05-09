# Phishing Website Detection with Machine Learning

## Overview
This project applies machine learning techniques to classify websites as either phishing or legitimate using a structured phishing website dataset. The project investigates how well different machine learning models perform on this cybersecurity task and analyzes which categories of features contribute most to predictive performance.

## Research Question
Can phishing websites be accurately detected using machine learning, and which feature groups are most useful for detection?

## Dataset
This project uses the **Web page Phishing Detection Dataset** from Kaggle:

[Web page Phishing Detection Dataset](https://www.kaggle.com/datasets/shashwatwork/web-page-phishing-detection-dataset)

The dataset contains 11,430 samples and 89 columns, including a binary target label (`status`) indicating whether a website is phishing or legitimate.

## Project Structure
```text
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

