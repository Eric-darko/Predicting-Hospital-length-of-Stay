Predicting Hospital Length of Stay

Overview

This project aims to predict the length of stay (LOS) for patients in hospitals using machine learning classification models. Accurate predictions of patient LOS can significantly enhance hospital resource allocation, improve patient care, and streamline operational processes. By identifying the expected duration of a patient's stay, healthcare facilities can optimize bed utilization and staffing requirements.

Technologies Used

Programming Language: Python
Jupyter Notebooks: For interactive coding and data visualization
Database: PostgreSQL for data storage and retrieval

Libraries:

scikit-learn: For building and evaluating machine learning models
pandas: For data manipulation and preprocessing
NumPy: For numerical operations
Matplotlib & Seaborn: For visualizations and exploratory data analysis

Data Source

The main data for this project was MIMIC-III (Medical Information Mart for Intensive Care III), which is a large freely accessible database that contains deidentified health-related data from over 50,000 patients who were admitted to the Beth Israel Deaconess Medical Center's critical care units between 2001 and 2012.(11) The data was acquired by taking a credentialled access course called the data and specimen research, access was granted to the database via PhysioNet, a resource for sharing physiological data and clinical recordings. The database consists of 26 tables with varying data types and information including:
Demographic data: This includes information such as the age, gender, ethnicity, and marital status of the patients.. It contains various features related to patient demographics, medical history, and treatment details that are crucial for predicting the length of stay.

Workflow

Data Cleaning:

Preprocessing the dataset by handling missing values and outliers.
Normalizing and encoding categorical variables for model compatibility.
Feature Engineering:

Creation of relevant features that enhance the predictive power of the models, such as age, diagnosis codes, and prior hospital visits.
Modeling:

Built classification models to predict LOS using both 3-class and 4-class intervals. The models implemented include:
Logistic Regression,
Random Forest,
Support Vector Machine(SVM),
Gradient Booster,

Evaluation:

Performance metrics such as accuracy, precision, recall, and F1-score were used to evaluate model performance. The results indicated that:
Key Results
The Random Forest classifier emerged as the best-performing model, achieving an accuracy of 87%. This suggests that it effectively captures the complexity of the factors influencing a patient’s length of stay.

Suggestions for Improvement

Data Augmentation: Incorporate additional features such as social determinants of health to improve model accuracy.
Model Interpretability: Utilize SHAP (SHapley Additive exPlanations) values to better understand feature contributions to model predictions.

Future Development

Deployment: Implement a web application that allows healthcare providers to input patient data and receive real-time predictions on expected length of stay.
Integration: Explore integrating the model with hospital information systems (HIS) for automated predictions based on real-time patient data.
Advanced Modeling Techniques: Investigate the application of deep learning methods, such as recurrent neural networks (RNNs), to capture temporal patterns in patient data.
