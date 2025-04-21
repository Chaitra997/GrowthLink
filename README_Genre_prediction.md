**README FILE FOR MOVIE GENRE CLASSIFICATION**

**Project Title:** Movie Genre Classification

### **Objective:** The objective of this project is to build a machine learning model that classifies movies into their respective genres based on plot descriptions. This is a multi-class classification task that involves natural language processing (NLP) techniques to convert unstructured textual data into a structured format for training models.

**Dataset:** Genre Classification Dataset IMDb 

**A.  Dataset Preprocessing Steps:** 

1. Loading the Data: Text files were read and split using the delimiter.
2. DataFrames Creation: Pandas DataFrames were created for training, testing, and solution datasets.
3. Label Encoding: Genres were encoded using LabelEncoder to convert text labels into numeric format.
4. TF-IDF Vectorization: The movie descriptions were vectorized using Tf-idfVectorizer to create feature vectors.

**B.  Exploratory Data Analysis:**  

1. Checked for missing values and duplicates.
2. Verified distribution of genres in the training data.
3. Ensured test and train sets do not overlap in titles or IDs.

**C. Models:** 

1. Logistic Regression
2. Naive Bayes
3. Random Forest Classifier
4. Voting Classifier


**D.  Hyperparameter Tuning:** Used GridSearchCV to find optimal hyperparameters:

- **Logistic Regression**: Tuned C value.
- **Naive Bayes**: Tuned alpha.
- **Random Forest**: Tuned n\_estimators and max\_depth.

**E.  Model Evaluation Metrics:**  Evaluation was performed using:

1. Accuracy
2. Classification Report: Includes Precision, Recall, and F1-score.
3. Model Comparison Plot: Bar chart comparing accuracy of all models.

**F. Outcome:**

|MODEL |ACCURACY |
| :-: | :-: |
|Logistic Regression|0\.5945|
|Naive Bayes|0\.5092|
|Random Forest|0\.4704|
|Voting Classifier|0\.5303|








