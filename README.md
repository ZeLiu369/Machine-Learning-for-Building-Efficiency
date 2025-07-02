[paper link](https://drive.google.com/file/d/1nec7kmoh-vWJjw4cmFNR3aGPZRm8DWON/view?usp=sharing)


# Introduction
This repository contains the code and dataset used in our research to enhance the predictive accuracy of the Energy Star Score of buildings using advanced machine learning techniques. By focusing on the expansive NYC benchmarking dataset, our study leverages the Random Forest algorithm to outperform traditional methods like Gradient Boosting, addressing both the robustness against overfitting and the interpretability of the model.

# Project Description
The aim of this project was to explore machine learning algorithms to more effectively predict the Energy Star Score, a crucial metric for assessing a building's energy efficiency. Our research primarily involved:
-  Comparing the Random Forest and Gradient Boosting algorithms.
- Developing regression and classification models to predict the Energy Star Score.
- Analyzing and visualizing the NYC benchmarking data to uncover key predictors and their implications on energy efficiency.


# Key Findings
- Random Forest demonstrated superior performance over Gradient Boosting, particularly in handling overfitting.
- Detailed data preprocessing and robust feature engineering significantly enhanced model accuracy.
- Insights from the model can inform strategies to enhance building energy efficiencies across various urban contexts.




# Methods
Our methodology encompasses several critical steps tailored to enhance the prediction of building energy efficiency:

- Data Preprocessing: The NYC benchmarking dataset was cleaned and formatted to handle missing values, ensure correct data types, and remove irrelevant or sparse columns. This step improved data quality and usability for modeling.

- Feature Engineering: We engineered features to better capture the nuances of building energy usage, including transformations and interactions between different variables.

- Model Training: We compared multiple machine learning models, with a primary focus on Random Forest and Gradient Boosting, to identify the most effective algorithm for our data.

- Model Evaluation: Models were rigorously evaluated using cross-validation techniques to assess their performance and generalizability across different datasets.

- Hyperparameter Tuning: Extensive tuning of model parameters was conducted to optimize performance, focusing on reducing overfitting while maintaining high predictive accuracy.

## Random Forest Tree hyperparamater finding:
![error vs depth](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/652ac16f-d37c-419b-8b0c-ea9b8e632c30)
![min_sample_leaf_1](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/90f05749-ce57-4fa7-a566-5facab4376d1)

![min_sample_leaf_2](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/a1bf7abf-cdac-402f-b5f1-2f5c7a43c243)
![min_sample_4](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/cec072b4-1da1-44c1-81e6-66b15964739a)
![min_samples_split](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/08fa68bb-0697-4c7b-8827-618fa843d1f4)
![feature_importance](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/9291e84e-48ed-4461-830c-318f54b47079)

# Results
The results of our study indicated several key findings:

- Performance Comparison: The Random Forest algorithm outperformed Gradient Boosting in terms of both accuracy and robustness against overfitting, making it the superior choice for this application.
- Feature Importance: Analysis of feature importance revealed that certain features, such as Site EUI and Weather Normalized Site Electricity Intensity, are critical predictors of the Energy Star Score. This insight can direct efforts towards variables most impactful for improving energy efficiency.

- Predictive Accuracy: The final Random Forest model demonstrated excellent predictive accuracy with a well-balanced approach to generalization, as evidenced by its performance metrics on the test and validation datasets.

- Insights for Building Efficiency: The model's predictions provide valuable insights into energy usage patterns and efficiency strategies, suggesting targeted areas for intervention to enhance building performance.


# Use LIMA
![tree](https://github.com/ZeLiu369/Machine-Learning-for-Building-Efficiency/assets/90260431/389c8f0e-e40e-42da-88bb-a5cba1aafaae)

In our study, we utilized LIME to provide insights into the individual predictions made by our machine learning models, enhancing the interpretability and trustworthiness of our results. LIME allowed us to deconstruct the complex decision-making processes of the Random Forest model, offering a granular view of how various features influenced the Energy Star Score predictions. By perturbing input data around specific instances and observing the changes in output, LIME generated explanations that were not only comprehensible but also highly informative. This technique proved invaluable in validating the influence of key features such as Site EUI and Weather Normalized Site Electricity Intensity on model predictions. Furthermore, LIME helped identify any potential biases or inconsistencies in the model, ensuring that our predictive framework was both robust and transparent, thereby enabling stakeholders to make informed decisions based on reliable, interpretable data.
