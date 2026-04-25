# End_to_End_Data_Analysis_and_Model_Build

📌 Project Overview
The system uses a dataset containing various parameters that influence crop growth. The model analyzes these features to predict the optimal crop from 22 different categories (including rice, maize, chickpeas, kidney beans, etc.).

📊 Dataset Features
The model is trained on the following soil and environmental attributes:

Nitrogen (N): Ratio of Nitrogen content in soil.

Phosphorus (P): Ratio of Phosphorous content in soil.

Potassium (K): Ratio of Potassium content in soil.

Temperature: Air temperature in degrees Celsius.

Humidity: Relative humidity in percentage.

pH: Soil pH value.

Rainfall: Rainfall in mm.

<img width="634" height="228" alt="image" src="https://github.com/user-attachments/assets/e7f77d1f-2751-4dd9-aff1-60086e9c49af" />


🛠️ Technical Implementation
1. Data Preprocessing
Handling Outliers: Used the Interquartile Range (IQR) method to clip extreme values.

Scaling: Implemented StandardScaler to normalize feature values for better model convergence.

Encoding: Used LabelEncoder for target crop labels.

2. Feature Engineering
Ratios: Calculated N/P, P/K, and N/K ratios to capture nutrient balance.

Statistical Features: Added NPK mean and standard deviation for each record.

Polynomial Features: Generated 2nd-degree interaction features to capture non-linear relationships between variables.

3. Machine Learning Models
The project evaluates several classification algorithms:

Logistic Regression (Achieved 98.64% Test Accuracy)

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest Classifier

Gradient Boosting

XGBoost Classifier

🚀 Model Performance
The models demonstrate high precision and recall, particularly Logistic Regression, which achieved:

Training Accuracy: 98.92%

Testing Accuracy: 98.64%

Weighted F1-Score: 0.99

📈 Visualizations
The project includes several diagnostic plots to evaluate performance:

Confusion Matrices: To visualize prediction errors across different crop classes.

t-SNE Visualizations: To project high-dimensional data into 2D space, demonstrating how the model clusters different crop types.


<img width="658" height="603" alt="image" src="https://github.com/user-attachments/assets/2d8904a7-cfcd-4884-88d6-c9d2f2307722" />

<img width="772" height="680" alt="image" src="https://github.com/user-attachments/assets/ffefe263-c0b6-4765-b881-99805c88f0b1" />



