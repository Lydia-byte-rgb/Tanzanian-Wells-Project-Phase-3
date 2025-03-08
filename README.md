# Tanzania Water Wells Classification Project
# Business Understanding
Access to clean and functional water sources is crucial for public health, agriculture, and economic development in Tanzania. Many rural communities rely on water wells, but many of these wells become non-functional due to poor maintenance, inadequate infrastructure, or environmental conditions. Efficient resource allocation and proactive maintenance can significantly improve water accessibility and sustainability.
# Business Understanding
Access to clean and functional water sources is crucial for public health, agriculture, and economic development in Tanzania. Many rural communities rely on water wells, but many of these wells become non-functional due to poor maintenance, inadequate infrastructure, or environmental conditions. Efficient resource allocation and proactive maintenance can significantly improve water accessibility and sustainability.
## Goal:
Predict the functionality of water wells in Tanzania using machine learning classification models.
## Goal:
Predict the functionality of water wells in Tanzania using machine learning classification models.## Objectives
This study aims to develop a predictive machine learning model to classify water wells as functional, non-functional, or in need of repair. The insights will support efficient resource allocation, maintenance planning, and sustainable water management.

Key Objectives
1. Develop and compare multiple machine learning classification models to determine the best-performing approach for predicting well functionality.
2. Identify the most influential factors affecting well status, including water source, infrastructure, management, and payment system.
3. Detect patterns in well failures to help government agencies, NGOs, and local communities allocate resources efficiently.
4. Provide actionable insights to improve water infrastructure and well maintenance strategies based on predictive modeling results.

## Research Questions
1. Which machine learning classification model provides the highest accuracy in predicting well functionality?
2. How well can the model differentiate between functional, non-functional, and repair-needed wells?
3. What are the most significant factors that influence whether a well is functional, non-functional, or in need of repair?
4. How do infrastructure-related factors like extraction type, well age, and management type affect well performance?
5. Do certain geographic locations or regions have a higher concentration of non-functional wells?
6. How can machine learning predictions be used to prioritize well maintenance and repairs?
7. What strategies can be implemented to reduce well failures and improve sustainable water access?
## Stakeholders & Beneficiaries
- Government & Policy Makers: Use model predictions to prioritize funding and infrastructure improvements.
- Non-Governmental Organizations (NGOs): Identify regions most in need of water infrastructure investments.
- Community Water Management Committees: Plan preventive maintenance strategies based on well failure risks.
- Local Engineers & Planners: Use insights from the model to optimize well construction & repair decisions.

## Data Source
DrivenData. (2015). Pump it Up: Data Mining the Water Table. Retrieved [Month Day Year] from https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table.
# Data Analysis
Distribution of well functionality
![bd31f95b-b6ff-4eb7-9006-02e50bc46a0d](https://github.com/user-attachments/assets/14de59e4-10e8-4e03-a881-ff0934dba72a)


Well age Vs functionality
![6515ac54-c553-45a5-834e-3f935ab6561e](https://github.com/user-attachments/assets/e1c89877-32f9-482a-a884-4753c77d6f15)

Effect of Extraction type on well functionality 
![9dd32368-fbf7-4c80-9774-cc1166b13682](https://github.com/user-attachments/assets/fc1816cc-efbc-4f15-878b-1d01ddd8772b)
Proportion of well functionality by management type
![cbf91e10-28ec-4e92-83e4-f3dae5850f9b](https://github.com/user-attachments/assets/64f82824-36a7-4263-b4c6-eb4bb8b6d5ff)
# Preprocessing
encoding and scaling done
# Modeling
Logistic regression
![cbdd4e50-cffe-43a3-8aa6-677de25caca6](https://github.com/user-attachments/assets/60b0e84e-298f-4b31-87ac-7cec0d535a95)

#Decision Tree
![e582de0f-4a50-4014-b758-6f2176e7b613](https://github.com/user-attachments/assets/a300d105-4535-4fba-8c53-aea50603c053)

Random Forest
![7e15c354-9aaf-45e2-80f0-5676bf92bae8](https://github.com/user-attachments/assets/af4be67c-b4ac-487c-85ea-4c56d129fb38)

K-Nearest Neighbors (KNN)
![48b08baa-52b8-493b-aa16-d63ffd8f49ce](https://github.com/user-attachments/assets/a841db2d-788e-4073-a4e1-69c776bebe96)

SVM
![dd92ad77-ba54-4d67-8f5a-f329f4dc7e55](https://github.com/user-attachments/assets/0024f4c6-14a9-40ff-809b-87572ae774be)
Gradient Boosting Classifier
![eaef0d7f-9456-42e0-9d00-a9242796c94f](https://github.com/user-attachments/assets/d6ab142d-16ac-4a9b-a0a6-60add81ac362)

Naive Bayes
![e43aebd5-53a5-4db0-b795-e36149936780](https://github.com/user-attachments/assets/5ae42537-b1d5-4f07-a0ec-4bc4e827c6db)
Tuned Random Forest
![cda9a7b7-3e47-4a24-b4ef-206b51693df2](https://github.com/user-attachments/assets/a98c4abf-508a-4f3f-8f9d-c404567eac91)
# Model evaluation
The best performing model was the Tuned Random Forest Model, achieving an accuracy of 79.61%. It demonstrated strong classification ability, particularly for Class 0 (precision: 81%, recall: 88%), while Class 1 had lower recall (67%), indicating some misclassification of positive cases. The weighted F1-score of 0.79 suggests a good balance between precision and recall. While the model is well-optimized, improving Class 1 recall through class balancing, threshold tuning, or feature engineering could further enhance performance.
# Conclusions
This study successfully developed and evaluated multiple machine learning models to predict the functionality of water wells, with the Tuned Random Forest Model emerging as the most accurate, achieving 79.61% accuracy. The findings reveal that key factors influencing well functionality include water source, infrastructure type, management system, and payment method. Patterns in well failures indicate that certain regions experience higher rates of non-functional wells, emphasizing the need for targeted intervention. The model’s ability to differentiate between functional, non-functional, and repair-needed wells provides valuable insights for optimizing maintenance and resource allocation.
# Recommendations
1. Adopt the Random Forest Model for Decision-Making: Government agencies and NGOs can integrate the trained model into decision support systems to guide maintenance scheduling and resource allocation.
2. Improve Data Collection and Feature Engineering: Enhancing the dataset with real-time sensor data, water quality metrics, and seasonal variations could improve model accuracy and predictive power.
3. Prioritize Maintenance for High-Risk Wells: The model’s predictions should be used to identify and prioritize high-risk wells in regions with a high concentration of non-functional or repair-needed wells.
4. Enhance Management and Payment Systems: Since management and payment structures influence well functionality, implementing more sustainable financing models (e.g., community-based funds or government subsidies) could help maintain water infrastructure.
5. Expand Geographic and Temporal Analysis: Further research should explore regional variations and long-term trends to understand how environmental and socio-economic factors impact well performance.
6. Continuous Model Optimization: Regular model retraining with newly collected data will ensure that the predictions remain accurate and relevant, adapting to evolving well conditions.
7. By leveraging machine learning for predictive maintenance, stakeholders can improve water well sustainability, reduce failures, and enhance water access for communities

    Jupyter notebook link
For further reference, the jupyter notebook can be accessed here:
 (https://github.com/Lydia-byte-rgb/Tanzanian-Wells-Project-Phase-3.ipynb)

# Contact information
For any clarification reach out to me on: lydiamangoa10@gmail.com

# Repository structure
README.md
phase_3_project.ipynb
