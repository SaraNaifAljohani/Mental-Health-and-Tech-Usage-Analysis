# Mental Health and Tech Usage Dataset Analysis

## 🚀 Project Overview
This project investigates the intricate relationship between mental health and technology usage. We applied a variety of machine learning techniques, including **regression**, **classification**, **clustering**, and **anomaly detection**, to analyze a dataset focused on digital behavior and its impact on well-being. The primary goal was to explore how factors like screen time, social media use, sleep, and physical activity relate to mental health indicators and stress levels.

## 🧠 Research Questions
Our analysis was guided by the following research questions:
* How does technology usage affect an individual's mental health status?
* Can specific behaviors, such as gaming or screen time hours, be predicted for a given age group?
* Are there common characteristics among individuals who report high stress levels?

## 📊 Dataset
The study utilized the **Mental Health and Technology Usage Dataset**, a structured dataset containing 6,635 records and 14 variables sourced from Kaggle.

The dataset was preprocessed to ensure quality and reliability, which included:
* **Data Cleaning:** All columns were found to have consistent data types and no missing or duplicate values were identified.
* **Normalization:** Numerical variables were normalized using Min-Max Scaling to ensure all features contributed equally to the models.
* **Categorical Encoding:** Categorical features were encoded to prepare the data for machine learning models.

---

## 💻 Methodology & Models
We employed a diverse range of machine learning methodologies:
* **Regression Analysis (Linear & Non-Linear):** Used to test for relationships between age and technology usage, as well as various variables and stress levels.
* **Classification:** We used four different classifiers to predict mental health indicators and stress levels.
    * **Decision Tree:** Classified stress into low vs. medium/high.
    * **Random Forest:** Predicted stress levels across three classes: low, medium, and high.
    * **Logistic Regression:** Explored the relationship between technology usage, stress, and online support usage.
    * **Support Vector Classifier (SVC):** Classified mental health status based on lifestyle and support features.
* **Clustering (K-Means & Hierarchical):** Unsupervised learning methods used to identify distinct user groups based on behavioral patterns.
* **Anomaly Detection:** Used to identify unusual behavioral patterns in the dataset with methods like Z-Score, IQR, Isolation Forest, and One-Class SVM.

---

## 📈 Key Findings & Limitations

### Findings
* **Regression models showed poor performance** (R² values were less than zero), indicating that age cannot reliably predict technology usage or stress outcomes.
* **Classification models achieved modest accuracy** (25-51%). The Decision Tree model identified **sleep hours, gaming hours, and social media usage** as key predictors of stress.
* **Clustering analysis provided interpretable insights**. Hierarchical Clustering revealed meaningful groupings based on access to support systems and mental health status, whereas K-Means primarily separated users based on gaming behavior.
* **Anomaly detection** successfully identified unusual behavioral patterns, though these were not directly linked to mental health outcomes.

### Limitations
The study's findings were constrained by several key limitations:
* **Dataset Quality:** The dataset's complexity, overlapping variables, and potential for being randomly generated raised concerns about its reliability.
* **Missing Variables:** Crucial confounding variables that influence mental health (e.g., chronic illness, socioeconomic background, personality traits) were absent from the dataset, which impacted the predictive power of the models.
* **Model Performance:** Most models produced weak to moderate results, suggesting that the conclusions should be considered exploratory and not definitive.

## 💡 Conclusion
The analysis highlights the complexity of predicting mental health outcomes from technology usage alone. While behavioral features may relate to mental health, they are insufficient for reliable prediction without more comprehensive data and advanced modeling approaches. The study's findings provide tentative insights into how digital behavior and support systems may relate to mental well-being and stress.