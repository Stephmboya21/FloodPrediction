# FloodPrediction
This project aims to predict the probability of flooding using various environmental and anthropogenic factors. The dataset contains 50,000 observations with multiple features such as Monsoon Intensity, Deforestation, Urbanization, River Management, and more. The target variable, FloodProbability, is a continuous variable that represents the likelihood of flooding in different regions.

The key goal of this project is to build a Linear Regression Model to predict FloodProbability based on these features. Before building the model, thorough Exploratory Data Analysis (EDA) was conducted to understand the data, identify patterns, and ensure the dataset is clean and ready for modeling.

### Project Motivation
Floods are among the most destructive natural disasters, and they can be influenced by both natural and human-driven factors. Predicting flood risk is critical for disaster preparedness and mitigating damage. The goal of this project is to use a dataset containing various environmental factors to predict flood probability using a linear regression model. By identifying the key factors that increase flood risk, we aim to help policymakers, urban planners, and environmental agencies better manage flood risk.

### Exploratory Data Analysis (EDA)
Before building the regression model, we conducted an in-depth Exploratory Data Analysis (EDA) to better understand the structure of the dataset and uncover any potential issues. The main steps of the EDA included:

Missing Values: No missing values were detected in the dataset, so no imputation was required.

Summary Statistics: Generated summary statistics to understand the distribution of variables. The variables showed reasonable ranges, though certain features like Urbanization and MonsoonIntensity had slightly higher variances.

Correlation Analysis: A correlation matrix was computed to check for relationships between features and multicollinearity. Features like Deforestation and Urbanization had strong correlations with FloodProbability.

### Data Visualization:

KDE Plots: Kernel Density Estimation (KDE) plots were used to serve the distribution of each feature and identify potential outliers.

ob![kde plot](https://github.com/user-attachments/assets/f408aac8-4a9e-450e-a2be-b287271bbff2)

Heatmap: A heatmap of the correlation matrix was used to visualize relationships between variables.

![heatmap](https://github.com/user-attachments/assets/d7e59c00-a7bd-4753-9220-2cc58ea0d51b)


### Key Insights from EDA:

TopographyDrainage, RiverManagement, and DeterioratingInfrastructure are strong indicators of flood probability.
The dataset does not suffer from multicollinearity based on the correlation matrix.
Features like Encroachments and CoastalVulnerability showed weak correlation with the target variable.

### Linear Regression Modeling
After conducting EDA, we built a Linear Regression Model to predict FloodProbability. Key steps included:

Data Preprocessing:

The dataset was split into training (80%) and test (20%) sets.
Model Training:

A LinearRegression model was fitted to the training data.
Evaluation:

Predictions were made on the test set, and performance was evaluated using Mean Squared Error (MSE) and R-squared (R²) to assess model accuracy.

### Evaluation Results:

MSE: The model had a mean squared error of 6.802384563575717e-33.
R²: The R-squared value was 1.0, indicating how well the model explains the variance in FloodProbability.

