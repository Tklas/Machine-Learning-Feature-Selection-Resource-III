# Machine Learning: Feature Selection Methods

## Project Overview

This project documents my practical learning and implementation of feature selection methods in Machine Learning. The work was based on a lesson I studied through instructional videos, supported by personal notes and practical exercises using Python.

The project helped me understand how selecting relevant features can simplify a machine learning model, reduce unnecessary complexity, and potentially improve predictive performance.

## Project Objectives

The main objectives of this project were to:

* Understand the importance of feature selection in machine learning.
* Explore different methods of identifying relevant features.
* Apply feature selection techniques using Python.
* Train and evaluate a machine learning model using selected features.
* Compare model performance using the weighted F1-score.
* Develop practical experience working with machine learning libraries and datasets.

## Dataset

For this practical exercise, I used the **Wine dataset** available through Scikit-learn.

The dataset contains measurements of different chemical properties of wine samples, which can be used to classify the samples into their respective classes.

The dataset was loaded into a Pandas DataFrame for exploration, visualization, and preparation before model training.

## Feature Selection Methods Implemented

I explored and implemented the following feature selection techniques:

### 1. Variance-Based Feature Selection

This method examines how much each feature varies across the dataset. Features with very low variance may provide limited information for distinguishing between classes.

I examined feature variance, applied Min-Max scaling, visualized the results, and evaluated model performance after removing selected features.

### 2. SelectKBest

SelectKBest selects a specified number of features based on a scoring function.

I used `mutual_info_classif` to evaluate the relationship between individual features and the target variable. I then examined different numbers of selected features and compared their model performance.

### 3. Recursive Feature Elimination (RFE)

Recursive Feature Elimination works by repeatedly removing less important features and evaluating the remaining features.

I applied RFE to investigate how the number of selected features affected the performance of the machine learning model.

### 4. Boruta Feature Selection

Boruta is a feature selection method used to identify relevant features by comparing their importance with that of randomized features.

I applied Boruta to the dataset and evaluated the resulting model using the weighted F1-score.

## Machine Learning Model

I used the `GradientBoostingClassifier` from Scikit-learn to train and evaluate the classification model.

The dataset was divided into training and testing sets using `train_test_split`.

I established a baseline model using all available features before applying feature selection techniques. This provided a reference point for evaluating the effects of feature selection.

## Model Evaluation

The primary evaluation metric used in this project was the **weighted F1-score**.

The weighted F1-score combines precision and recall while accounting for the number of samples in each class.

The baseline model, trained using all features, achieved a weighted F1-score of **0.908**.

After applying the different feature selection methods, I compared their performance to understand how selecting features influenced the model's classification results.

The Boruta-based model achieved a weighted F1-score of **0.982** in my practical implementation.

These results illustrate how feature selection can affect model performance, although the best approach depends on the dataset, selected features, and evaluation setup.

## Tools and Technologies

The following Python libraries and tools were used:

* **Python** — programming language used for the practical implementation.
* **Pandas** — data manipulation and analysis.
* **NumPy** — numerical operations.
* **Matplotlib** — data visualization.
* **Seaborn** — visualization of feature distributions.
* **Scikit-learn** — dataset loading, data splitting, feature selection, model training, and evaluation.

## Key Learnings

Through this exercise, I developed a better understanding of:

* Why feature selection is an important part of the machine learning workflow.
* How different feature selection techniques identify relevant features.
* How to establish a baseline model for performance comparison.
* How to use the weighted F1-score to evaluate a classification model.
* How the number and selection of features can influence predictive performance.
* Why model evaluation is important when deciding which feature selection method to use.

I also gained practical experience implementing the methods in Python and reproducing the lesson's exercises in my own script.

## Project Files

The repository contains the following project materials:

* `Student_Resource_111.ipynb` — Jupyter Notebook containing the practical implementation and analysis.
* `feature_selection.py` — Python script containing the practical work.
* `Machine_Learning_Lesson_Report.docx` — documentation of my learning process, understanding, and key takeaways.

## Conclusion

This project strengthened my understanding of feature selection and its role in building machine learning models.

By implementing and comparing variance-based selection, SelectKBest, Recursive Feature Elimination, and Boruta, I gained practical insight into different approaches to selecting relevant features and evaluating their effects on model performance.

The exercise also reinforced the importance of experimentation, performance evaluation, and choosing an appropriate method based on the problem being solved.

# Video Presentation

This video presentation provides an overview of my learning and practical implementation of feature selection methods in machine learning.

Watch the presentation: [https://drive.google.com/file/d/1IQ2pNvBf8X-Emr7xcN37vetWkpJ8r7FW/view?usp=drive_link]

**Project Area:** Machine Learning
**Topic:** Feature Selection Methods
**Language:** Python
**Status:** Completed practical exercise
