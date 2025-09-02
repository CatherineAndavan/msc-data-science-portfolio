These notebooks showcase three distinct machine learning projects: classification, regression, and Natural Language Processing (NLP). Each project tackles a different problem, demonstrating a complete workflow from data preprocessing to model evaluation.

1. Classification (Injury Severity Prediction)
Goal: Predict the severity of a person's injury using the Fatality Analysis Reporting System (FARS) dataset.

Approach:

Preprocessed data by applying one-hot encoding to categorical features and standardization to numerical features.

Trained and evaluated Decision Tree and Random Forest classifiers.

Results: Considering the results of the four pipelines, Pipeline 2, which employed a Random Forest Classifier provided the best results.

2. Regression (Bacteria Growth Prediction)
Goal: The regression project aims to predict the growth of bacteria by building machine learning models.

Approach:

The notebook checks for data types and null values in the dataset.

It uses LinearRegression, SVR, and RandomForestRegressor to build and compare models.

Results: The results show that the Random Forest model performed the best.

3. NLP (News Article Topic Modeling)
Goal: Identify and cluster news articles by their underlying topics.

Approach:

Preprocessed text data by converting it to lowercase, removing punctuation, and applying stop word removal and stemming. The processed text is then vectorized using TF-IDF.

Implemented and compared two unsupervised models: LDA (Latent Dirichlet Allocation) and Agglomerative Clustering.

Results: LDA is the better option as it produced more defined clusters with less overlap. Using different preprocessing techniques or more complex models like CNNs could improve the results.

Skills & Tools
Python, Pandas, Scikit-learn, TensorFlow, NLTK, Matplotlib, Data Preprocessing, Feature Engineering, Classification, Regression, Natural Language Processing, Topic Modeling, Supervised Learning, Unsupervised Learning.
