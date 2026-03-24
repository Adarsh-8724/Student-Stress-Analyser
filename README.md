# Student-Stress-Analyser
Here is a structured, professional `README.md` file tailored to your notebook. You can copy and paste this directly into your GitHub repository.

-----

# 🎓 Student Stress Analyser

### Analysis and Prediction of Student Academic Stress Levels

Academic stress is a growing concern that significantly impacts both student performance and mental well-being. This project implements an end-to-end Data Science pipeline to analyze key lifestyle and academic factors contributing to student stress and utilizes Machine Learning to predict stress levels.

This project was developed as part of the Project-Based Learning (PBL) curriculum for the Introduction to Data Science course.

-----

## 📑 Table of Contents

  * [Project Overview](https://www.google.com/search?q=%23project-overview)
  * [Dataset](https://www.google.com/search?q=%23dataset)
  * [Machine Learning Pipeline](https://www.google.com/search?q=%23machine-learning-pipeline)
  * [Models Evaluated](https://www.google.com/search?q=%23models-evaluated)
  * [Key Insights & Results](https://www.google.com/search?q=%23key-insights--results)
  * [Ethics & Limitations](https://www.google.com/search?q=%23ethics--limitations)
  * [Author](https://www.google.com/search?q=%23author)

-----

## 🎯 Project Overview

The primary objectives of this project are to:

1.  Conduct comprehensive **Exploratory Data Analysis (EDA)** to uncover patterns between student lifestyle and stress.
2.  Build, evaluate, and compare multiple machine learning classifiers.
3.  Classify student stress levels into three distinct categories: `Low`, `Medium`, and `High`.
4.  Critically evaluate the ethical dimensions and potential biases of using predictive models for mental health analysis.

-----

## 📊 Dataset

**Source:** [Student Stress Factors Extended Dataset (Kaggle)](https://www.kaggle.com/datasets/rxnach/student-stress-factors-extended-dataset)

The dataset consists of survey responses where students rated various factors on a scale of 1 to 5.

**Features:**

  * `sleep_quality`: Quality and duration of sleep.
  * `headache_frequency`: How often the student experiences headaches.
  * `academic_performance`: Self-rated academic standing.
  * `study_load`: Perceived weight of academic coursework.
  * `extracurricular_activities`: Involvement in activities outside of academics.

**Target Variable:** \* `stress_level` (Categorized into `Low`, `Medium`, and `High`)

-----

## ⚙️ Machine Learning Pipeline

1.  **Data Preprocessing:** Handled missing values, checked for duplicates, and verified bounded outliers using the IQR method.
2.  **Feature Engineering:** Mapped numerical stress scores to categorical labels and scaled feature matrices using `StandardScaler`.
3.  **Exploratory Data Analysis:** Generated statistical summaries, correlation heatmaps, feature distributions, and pairplots using `matplotlib` and `seaborn`.
4.  **Model Training:** Split data using an 80/20 stratified split and trained models using 5-fold cross-validation.
5.  **Hyperparameter Tuning:** Optimized the best-performing model using `GridSearchCV`.

-----

## 🤖 Models Evaluated

Six different classification algorithms were trained and compared based on accuracy and cross-validation scores:

  * Logistic Regression
  * Decision Tree Classifier
  * Random Forest Classifier 🏆 *(Best Performing)*
  * K-Nearest Neighbors (KNN)
  * Support Vector Machine (SVM)
  * Gradient Boosting Classifier

-----

## 📈 Key Insights & Results

After hyperparameter tuning, the **Random Forest Classifier** emerged as the most accurate model.

**Core Findings:**

  * **Sleep Quality** and **Study Load** are the most significant predictors of academic stress.
  * Students reporting poor sleep quality consistently fell into the `High` stress category.
  * Regular participation in extracurricular activities serves as a notable stress buffer.

-----

## ⚖️ Ethics & Limitations

Responsible AI development requires acknowledging the limitations of our models:

  * **Subjectivity:** The dataset relies on self-reported Likert scales, meaning the perception of a "5" in stress can vary wildly between two different students.
  * **Scope:** The model does not account for critical external factors such as financial stability, genetic predispositions, or family dynamics.
  * **Intended Use:** This tool is designed for exploratory data analysis and early-warning assistance, and must **never** replace professional medical or psychiatric diagnosis. Mental health data requires strict privacy and informed consent protocols.

-----

## 👨‍💻 Author

**Adarsh**

  * **Program:** B.Tech Computer Science and Engineering (CSE) - Specialization in AI/ML (in collaboration with IBM ICE)
  * **University:** IILM University, Greater Noida

-----

Would you like me to also write a `requirements.txt` file listing the exact libraries (pandas, scikit-learn, seaborn, etc.) needed to run your notebook?
