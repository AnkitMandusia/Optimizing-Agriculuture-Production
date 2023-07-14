# Optimizing-Agriculuture-Production


**Objective:** To develop predictive models for crop yield prediction and fertilizer recommendation. By leveraging machine learning techniques, the project aims to optimize agricultural production by accurately predicting crop yields and providing personalized fertilizer recommendations based on specific climatic and soil conditions.

**Goal:** The goal of the project is to enhance agricultural practices and increase productivity by leveraging data-driven approaches. Specifically, the project aims to achieve the following:

1. **Crop Yield Prediction:** Develop a model that can accurately predict crop yields based on relevant environmental factors such as temperature, humidity, rainfall, soil nutrients (Nitrogen, Phosphorus, Potassium), and pH levels. The goal is to provide farmers with insights into expected crop yields, enabling them to make informed decisions regarding planting strategies, resource allocation, and crop management.

2. **Fertilizer Recommendation:** Build a model that recommends suitable fertilizer types and quantities for different crops based on their specific nutrient requirements and the existing soil conditions. By analyzing the soil nutrient levels and crop-specific nutrient needs, the goal is to optimize fertilizer usage and minimize waste while ensuring optimal crop growth and productivity.


Data Collection: The data for the project has been collected from a public dataset available on Kaggle. It is important to mention the specific dataset you used and provide its proper citation or link to acknowledge the source.
Exploratory Data Analysis (EDA): The code snippet includes an EDA section where various visualizations are created to analyze the dataset. This is an important step to gain insights into the data before building the models. Some key observations made from the visualizations include:

Different crops have varying nutrient requirements (e.g., Nitrogen, Phosphorus, Potassium).
Certain crops have specific climate preferences (e.g., hot climate for Papaya, humid climate for Coconut).
Chickpea requires high pH in the soil, while Rice requires a significant amount of rainfall.
These observations help in understanding the relationships between different features and the target variable (crop label). It provides valuable insights into the factors influencing crop growth and can guide the feature selection process for model building.

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/eae2ff65-e135-4a16-b29e-8671f62b01b8)

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/e45c3e1c-53d9-43ed-8d80-96543980d12e)

Model Building: The code snippet demonstrates the implementation of several classification models for crop prediction. Here are some key points related to model building:

K-Nearest Neighbors (KNN): The KNN algorithm is used with different values of k (number of neighbors) and cross-validation to find the optimal value. The performance of the model is evaluated using classification report and confusion matrix.
Support Vector Classifier (SVC): Randomized search cross-validation is employed to find the best hyperparameters for SVC. The resulting model is evaluated using the classification report.
Logistic Regression: Randomized search cross-validation is used to optimize the hyperparameters for Logistic Regression. The performance of the model is evaluated using the classification report.
Random Forest Classifier: Randomized search cross-validation is performed to find the optimal number of estimators for the Random Forest model. The resulting model is evaluated using the classification report.
LightGBM Classifier: The LightGBM classifier is trained on the data, and its performance is evaluated using the classification report. The model achieves 100% accuracy in this case.


