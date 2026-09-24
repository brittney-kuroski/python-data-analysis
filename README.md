# Predictors of Sleep Disorders

## 📊 Project Overview

Can we predict whether an individual is likely to have a sleep disorder based on factors such as **BMI, stress level, and sleep quality**?

This project uses exploratory data analysis and logistic regression to investigate relationships between lifestyle and health-related factors and the presence of a sleep disorder.

The goal was to build a classification model that could predict whether an individual **has a sleep disorder or does not have a sleep disorder**.

---

## 🎯 Research Question

**Could we accurately predict the likelihood of a sleep disorder based on a person's BMI, stress level, and sleep quality?**

---

## 📁 Dataset

The dataset was sourced from **Kaggle** and contains information on 374 adults between the ages of 27 and 59.

The original dataset contains both numerical and categorical variables.

**Dataset shape:** 374 rows × 13 columns

The analysis focused on variables relevant to predicting the presence of a sleep disorder.

---

## 🧹 Data Preparation

Before building the model, the data was prepared for analysis by:

* Removing data that was not needed for the analysis
* Normalizing BMI categories
* Converting categorical variables into numerical/binary representations
* Converting **Gender**, **Quality of Sleep**, **Stress Score**, and **Sleep Disorder** into binary columns
* One-hot encoding the **BMI Category** variable

These transformations allowed the categorical information to be incorporated into the logistic regression model.

---

## 🔎 Exploratory Data Analysis

A correlation matrix was used to explore relationships between the variables.

One notable finding was the relationship between BMI category and sleep disorder status:

* A **Normal BMI** category showed a negative correlation with having a sleep disorder.
* An **Overweight BMI** category showed a positive correlation with having a sleep disorder.

These relationships helped inform the variables used in the predictive model.

---

## 🤖 Machine Learning Model

### Logistic Regression

A **Logistic Regression** model was selected because the target variable contains two possible outcomes:

* **Has a sleep disorder**
* **Does not have a sleep disorder**

The model was trained and evaluated using a test dataset.

---

## 📈 Model Results

The model correctly predicted the presence or absence of a sleep disorder in **91% of the test cases**.

### Confusion Matrix

|                         | Predicted: No Disorder | Predicted: Disorder |
| ----------------------- | ---------------------: | ------------------: |
| **Actual: No Disorder** |                     40 |                   3 |
| **Actual: Disorder**    |                      3 |                  23 |

The model correctly classified:

* **40** individuals without a sleep disorder
* **23** individuals with a sleep disorder

It incorrectly classified **6** individuals.

The classification report also showed balanced performance across the two classes.

---

## 💡 Key Takeaways

This analysis demonstrated that information related to BMI, stress, and sleep quality can be used to build a model for predicting the presence of a sleep disorder.

The logistic regression model achieved **91% accuracy on the test dataset**, while maintaining relatively balanced performance between the two outcome classes.

This project provided experience with the complete data analysis process, including:

* Data cleaning and transformation
* Exploratory data analysis
* Feature preparation
* Classification modeling
* Model evaluation
* Communicating analytical findings

---

## 🛠️ Tools & Technologies

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Logistic Regression**
* **GitHub**

---

## 📂 Project Files

| File                                 | Description                                                                          |
| ------------------------------------ | ------------------------------------------------------------------------------------ |
| `Sleep_Sisorder_Analysis.ipynb`      | Jupyter Notebook containing the data preparation, analysis, modeling, and evaluation |
| `Sleep_Disorder_Dataset.csv`                 | Dataset used for the analysis                                                        |
| `Sleep_Disorder_Presentation.pptx` | Presentation summarizing the project, methodology, and findings                      |

---

## 👩‍💻 About This Project

This project was created as part of my development in **data analytics and data science**, with a focus on using data to answer questions, identify patterns, and communicate actionable insights.

**Author:** Brittney Kuroski
