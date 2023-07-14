
# Optimizing-Agriculuture-Production




## Objective
To develop predictive models for crop yield prediction and fertilizer recommendation. By leveraging machine learning techniques, the project aims to optimize agricultural production by accurately predicting crop yields and providing personalized fertilizer recommendations based on specific climatic and soil conditions.

## Goal
The goal of the project is to enhance agricultural practices and increase productivity by leveraging data-driven approaches. Specifically, the project aims to achieve the following:

1. **Crop Yield Prediction:** Develop a model that can accurately predict crop yields based on relevant environmental factors such as temperature, humidity, rainfall, soil nutrients (Nitrogen, Phosphorus, Potassium), and pH levels. The goal is to provide farmers with insights into expected crop yields, enabling them to make informed decisions regarding planting strategies, resource allocation, and crop management.

2. **Fertilizer Recommendation:** Build a model that recommends suitable fertilizer types and quantities for different crops based on their specific nutrient requirements and the existing soil conditions. By analyzing the soil nutrient levels and crop-specific nutrient needs, the goal is to optimize fertilizer usage and minimize waste while ensuring optimal crop growth and productivity.

## Data Collection
The data for the project has been collected from a public dataset available on Kaggle. It is important to mention the specific dataset you used and provide its proper citation or link to acknowledge the source.
## Exploratory Data Analysis (EDA)
 The code snippet includes an EDA section where various visualizations are created to analyze the dataset. This is an important step to gain insights into the data before building the models. Some key observations made from the visualizations include:

Different crops have varying nutrient requirements (e.g., Nitrogen, Phosphorus, Potassium).
Certain crops have specific climate preferences (e.g., hot climate for Papaya, humid climate for Coconut).
Chickpea requires high pH in the soil, while Rice requires a significant amount of rainfall.
These observations help in understanding the relationships between different features and the target variable (crop label). It provides valuable insights into the factors influencing crop growth and can guide the feature selection process for model building.

EDA For Crop Yields:
![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/bf517a45-cdb9-44eb-bcfe-4e8b59ac0a64)


![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/d416b313-5ff5-4646-909a-dfff99cbaf95)


EDA For Fertilizer:
![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/621d3047-79d7-45c1-a5c4-b076e2e9dbea)


## Model Building

Models for Crop Yield Prediction


**K-Nearest Neighbors (KNN)**

The KNN algorithm is used with different values of k (number of neighbors) and cross-validation to find the optimal value. The performance of the model is evaluated using classification report and confusion matrix.

**Support Vector Classifier (SVC)**

 Randomized search cross-validation is employed to find the best hyperparameters for SVC. The resulting model is evaluated using the classification report.

**Logistic Regression**

 Randomized search cross-validation is used to optimize the hyperparameters for Logistic Regression. The performance of the model is evaluated using the classification report.

**Random Forest Classifier** Randomized search cross-validation is performed to find the optimal number of estimators for the Random Forest model. The resulting model is evaluated using the classification report.

**LightGBM Classifier**

 The LightGBM classifier is trained on the data, and its performance is evaluated using the classification report. The model achieves 100% accuracy in this case.

**XGBoost Classifier**

 A pipeline is created using make_pipeline to apply feature scaling and train an XGBoost Classifier model. The accuracy on the test data and the whole data are evaluated and displayed. Finally, the trained model is pickled for future use.

## Model Evaluation

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/5ecf7abf-667b-4bca-9102-7ed85a036bfb)

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/d78a44e6-9334-41e3-a70a-373b3bf28145)


## Results
Crop Prediction

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/7724ab5c-f947-4e26-b4bf-ff8ae989b3cc)


Fertilizer Prediction

![image](https://github.com/AnkitMandusia/Optimizing-Agriculuture-Production/assets/53564761/7b7b14d2-a6d2-4ae1-b1b5-393bdf6b69ba)




## Future Scope


- Explore additional feature engineering techniques to capture more nuanced relationships between environmental factors, soil characteristics, and crop requirements.

- Conduct a more extensive search for optimal hyperparameter configurations for each model using techniques like grid search or Bayesian optimization.
- Consider customizing the models based on specific crops or regional variations to provide more personalized and accurate fertilizer recommendations.
- Augment the existing dataset with additional data from diverse sources to enhance the model's ability to capture complex relationships.
- Build a real-time monitoring system to continuously collect data and update recommendations based on evolving conditions.
- Develop an interactive and user-friendly interface or application for farmers to access the fertilizer recommendation system.
- Integrate the system with IoT devices and sensor technologies deployed in agricultural fields to leverage real-time data for more accurate recommendations.
