# Fetal Health Classification with Logistic Regression and Random Forest

## Overview

This project aims to classify fetal health conditions using machine learning techniques, specifically Logistic Regression and Random Forest algorithms. The dataset used for this project contains fetal health data from Cardiotocogram (CTG) exams. The goal is to predict the health status of a fetus—categorized as Normal, Suspect, or Pathological—based on various medical features extracted from the CTG data.

## Dataset

The dataset used in this project is publicly available on Kaggle. It contains 2126 samples with 21 features each, derived from CTG exams. The target variable (`fetal_health`) is categorized into three classes:
- 1: Normal
- 2: Suspect
- 3: Pathological

## Features

The dataset includes features such as:
- Baseline value (FHR baseline)
- Accelerations (Number of accelerations per second)
- Fetal movement (Number of fetal movements per second)
- Uterine contractions (Number of uterine contractions per second)
- ... and others.

These features are used as input to the machine learning models to classify the fetal health status.

## Models

### 1. Logistic Regression with Backward Selection
The Logistic Regression model is trained with a backward selection technique to eliminate insignificant variables, leading to a more robust and interpretable model.

### 2. Random Forest with Hyper-Parameter Tuning
The Random Forest model is trained with hyper-parameter tuning using Randomized Search CV to optimize the model's performance.

## Performance Metrics

Both models are evaluated using precision, recall, and F1-score. The Random Forest model generally outperforms Logistic Regression in terms of accuracy and overall F1-score.

## Installation and Setup

To run the code in this project, you need to have Python installed along with several key libraries. Follow the steps below to set up your environment:

1. **Clone the Repository** (assuming you have uploaded this project to GitHub):
   ```bash
   git clone https://github.com/yourusername/fetal-health-classification.git
   cd fetal-health-classification
