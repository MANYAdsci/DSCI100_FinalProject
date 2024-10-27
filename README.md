# Iris Species Classification

## Project Overview
This project aims to predict the species of the Iris flower using its sepal and petal dimensions. We use a machine learning classification approach to distinguish between three species: Iris setosa, Iris versicolor, and Iris virginica. The project involves data preprocessing, exploratory data analysis, model training using K-Nearest Neighbors (KNN), and accuracy evaluation.

## Group Members
- Manya Jain
- Zhuohang Lyu
- Chang Sun

## Dataset
The dataset used for this project is the "Iris Flower Dataset," also known as Fisher's Iris Dataset, which is available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris). The dataset consists of 150 observations with the following columns:
- `SepalLengthCm`: Length of sepal in centimeters.
- `SepalWidthCm`: Width of sepal in centimeters.
- `PetalLengthCm`: Length of petal in centimeters.
- `PetalWidthCm`: Width of petal in centimeters.
- `Species`: The species of Iris (Iris setosa, Iris versicolor, Iris virginica).

## Methodology
1. **Data Preprocessing**: The dataset is cleaned by removing unnecessary columns and converting the species column to a factor. The dataset is then split into training and testing sets (80-20 split).
2. **Exploratory Data Analysis (EDA)**: Visualization of data to observe relationships between different variables.
3. **Model Training**:
   - The K-Nearest Neighbors algorithm is used with three different models:
     - Using all four predictors (sepal and petal dimensions).
     - Using only sepal dimensions.
     - Using only petal dimensions.
   - Cross-validation is applied to determine the optimal number of neighbors (K).
4. **Model Evaluation**:
   - Accuracy of each model is computed.
   - A confusion matrix is used to understand the classification performance.
   - Results from different models are compared.

## Results
- The model using all four predictors and the one using only petal dimensions both achieved an accuracy of approximately 96%.
- The model using only sepal dimensions had a lower accuracy of around 76%.

## Visualizations
- Scatter plots are used to show relationships between sepal and petal dimensions.
- A comparison bar chart is provided to visualize the accuracy of different models.

## Expected Outcomes and Discussion
The findings suggest that petal dimensions are more effective for classification than sepal dimensions. The results could have implications for understanding the morphological differences between Iris species and their adaptation to different environments.

## Technologies Used
- R for data analysis and modeling
- Libraries: `tidyverse`, `tidymodels`, `ggplot2`
