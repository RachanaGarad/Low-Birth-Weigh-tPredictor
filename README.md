# Low-Birth-Weight Predictor

**Objective**
To predict low birth weight using a dataset containing a variety of maternal and paternal factors, employing machine learning techniques to develop an accurate predictive model.

**Introduction**
This project aims to analyze and predict low birth weight using a comprehensive dataset that includes significant variables such as maternal age, maternal education, prenatal care visits, paternal age, paternal education, cigarette consumption during pregnancy, alcohol consumption during pregnancy, gender, and ethnicity indicators. The goal is to leverage these variables to develop a predictive model that can accurately estimate birth weight, facilitating better prenatal care and interventions​​.

**Analysis**
The analysis involves several steps:

Exploratory Data Analysis (EDA): Understanding the distribution of variables, identifying trends, and evaluating missing values.
Feature Engineering: Creating new features and refining existing ones to improve model performance. For instance, developing a health behavior score based on cigarette and alcohol consumption during pregnancy, and a prenatal care index based on the number of prenatal visits and the month of pregnancy when prenatal care began​.
Model Development: Systematically creating and assessing multiple candidate models to identify the best-performing one for predicting birth weight.

**Technology
The project utilizes various tools and libraries for data manipulation, analysis, and visualization, including:

Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
Matplotlib: For data visualization​.

**Models Used**
Several models were evaluated for predicting low birth weight:

Logistic Regression: High accuracy for the majority class but struggled with identifying the minority class (low birth weight), leading to low recall and F1 scores​​.
Ridge Classifier: Showed slight improvement in recognizing low birth weight instances with better recall than Logistic Regression but still had several false negatives​​.
K-Nearest Neighbors (KNN) Classifier: Tendency to predict the majority class, with a high number of false negatives, leading to poor recall and low F1 score​​.
Decision Tree Classifier: More balanced approach between recognizing both classes with higher recall for low birth weight cases but lower precision​​.
Random Forest Classifier: Demonstrated relatively good performance with high accuracy and precision but moderate recall, indicating it still missed several true low birth weight instances​​.
Gradient Boosting Machine (GBM) Classifier: Moderate precision but low recall, indicating it missed many actual low birth weight cases​​.
**The KNN Classifier** was selected as the final model due to its balance between training and test accuracy, reflecting a smaller train-test gap and less overfitting compared to other models like Random Forest and Gradient Boosting​​.


**Results**
The results of the project highlight the importance of maternal age in prenatal care strategies. Visual analyses emphasize the need to tailor interventions for middle-aged expectant mothers, who exhibit a wider range of birth weights, thus addressing the factors contributing to this variability. The final predictive model effectively uses the engineered features to provide accurate estimations of birth weight, demonstrating the model's potential in aiding prenatal care planning and interventions.
