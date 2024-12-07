# Antoine Abou Faycal & Mahdi Alhakim
# EECE490 Hackathon

Welcome to the **EECE490 Hackathon** repository! This hackathon submission explores the behavioral patterns and economic influences on cigarette consumption among Lebanese smokers. By leveraging machine learning techniques—both supervised and unsupervised—this work aims to provide insights into how personality traits, economic hardship, and lifestyle factors correlate with smoking behavior, brand preferences, and brand switching patterns.

## Table of Contents

- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Data Description](#data-description)
- [Notebooks and Their Purpose](#notebooks-and-their-purpose)
- [Key Findings and Conclusions](#key-findings-and-conclusions)
- [Future Work and Potential Improvements](#future-work-and-potential-improvements)

---

## Project Overview

This project focuses on understanding and predicting cigarette consumption behaviors using demographic, personality, and economic factors. The overarching goals are:

1. **Classification of Cigarette Consumption**:  
   Predict whether a smoker belongs to a certain category of daily cigarette consumption based on personality traits, demographics, and stress levels.

2. **Clustering of Smokers**:  
   Segment smokers into distinct groups using K-Means clustering. This grouping aims to identify patterns that distinguish "low," "medium," and "extreme" smokers without using labeled outcomes.

3. **Brand Switching Prediction**:  
   Determine if the ongoing economic crisis in Lebanon influences smokers to switch from their preferred brands to more affordable alternatives.

By exploring multiple analytical avenues—classification, clustering, and predictive modeling—the project offers a holistic view of the factors shaping smoking behaviors.

---

## Repository Structure

- **`2024_PersonalityTraits_SurveyData.xls`**:  
  The primary dataset containing demographic, economic, lifestyle, personality traits, and smoking behavior responses.

- **`cigarette_consumption_prediction.ipynb`**:  
  A Jupyter notebook that builds and evaluates a Logistic Regression model to classify smokers into daily consumption categories based on various input features.

- **`kmeans_clustering.ipynb`**:  
  A Jupyter notebook implementing K-Means clustering to group smokers into distinct clusters. This unsupervised approach aims to reveal underlying structure and smoker profiles based on personality and demographic traits.

- **`brand_switching_prediction.ipynb`**:  
  A Jupyter notebook utilizing Logistic Regression to predict whether smokers have switched brands due to economic hardship. It examines the influence of economic conditions, income sufficiency, stress, and other psychosocial factors on brand-switching behavior.

---

## Data Description

The dataset **`2024_PersonalityTraits_SurveyData.xls`** includes:

- **Demographics**: Age, gender, education level, employment status, region of residence.
- **Economic Indicators**: Monthly household income, perceived sufficiency of income, degree of economic hardship.
- **Lifestyle Factors**: Frequency of exercise, stress levels, and changes in smoking habits post-economic crisis.
- **Personality Traits**: Responses to standardized personality inventory items (e.g., extraversion, conscientiousness, neuroticism, openness, agreeableness).
- **Smoking Habits**: Daily cigarette consumption levels, brand preferences, ability to afford preferred brands, and brand-switching behavior post-economic downturn.

---

## Notebooks and Their Purpose

1. **`cigarette_consumption_prediction.ipynb`**  
   - **Goal**: Build a Logistic Regression model to predict daily cigarette consumption categories.  
   - **Process**:
     - Data cleaning, handling missing values.
     - Categorical encoding of personality and demographic features.
     - Model training, evaluation, and confusion matrix visualization.
   - **Output**: Provides accuracy measures, a confusion matrix, classification report, and feature importance analysis.

2. **`kmeans_clustering.ipynb`**  
   - **Goal**: Identify natural groupings among smokers using K-Means clustering.  
   - **Process**:
     - Data preprocessing, handling of missing values, and encoding of categorical features.
     - Clustering into three groups (Low, Medium, Extreme).
     - PCA for dimensionality reduction and cluster visualization.
   - **Output**: A visual 2D PCA plot of clusters and a cluster characteristic summary, aiding interpretation of underlying smoker segments.

3. **`brand_switching_prediction.ipynb`**  
   - **Goal**: Predict whether smokers switched to alternative brands due to the economic crisis.  
   - **Process**:
     - Data preprocessing with one-hot encoding and scaling.
     - Logistic Regression model training with hyperparameter tuning.
     - Performance evaluation using accuracy, confusion matrices, and classification reports.
     - Model persistence (saving and loading the model) and demonstration of test case predictions.
   - **Output**: A trained predictive model along with insights into the key factors influencing brand switching.

---

## Key Findings and Conclusions

- **Personality Traits Matter**:  
  Certain personality dimensions (e.g., anxiety, openness, conscientiousness) showed correlation with cigarette consumption patterns and the propensity to switch brands.

- **Economic Hardship and Behavior Change**:  
  As income sufficiency and stability decrease, the likelihood of switching to cheaper cigarette brands increases. Stress and economic pressure shape not only the number of cigarettes smoked but also the chosen brand.

- **Distinct Smoker Segments**:  
  Clustering reveals that smokers can be segmented into distinct groups with unique demographic, personality, and consumption profiles. Understanding these segments can inform targeted health interventions or market strategies.

- **Predictive Modeling Feasibility**:  
  Logistic Regression models provided reasonable accuracy in both consumption classification and brand switching prediction. However, the performance can be further improved with more sophisticated techniques or enriched data.

---

**With this repository, we hope to contribute to a deeper understanding of how personality, economic factors, and societal pressures influence smoking behavior.**
