# raisin-data-classification
### Project Overview
The project focuses on raisin data classification, utilizing a binary classification technique to distinguish between two types of raisins: Kecimen and Besni. The workflow includes exploratory data analysis (EDA), feature engineering, preprocessing, and model training using Random Forest and Support Vector Machine (SVM) algorithms.
### Exploratory Data Analysis for Raisin Data Classification
Checking for Data Types:
Verified that numerical columns (Area, Perimeter, etc.) are correctly identified as numerical and the target variable (Class) as categorical.

Finding Missing Values:
Ensured dataset completeness by using methods like isnull() to confirm no missing values were present.

Outliers Analysis:
Used box plots to detect outliers and the IQR method to remove values lying beyond 1.5 times the IQR from the first and third quartiles.

Correlation Analysis:
Visualized the correlation matrix with a heatmap, where darker colors indicate stronger correlations, helping to identify significant feature relationships.

Dependent and Independent Variables:
Independent variables include features like Area and Perimeter, while the dependent variable is the Class (Kecimen or Besni).

Standardization and Normalization:
Standardized features to have a mean of 0 and a standard deviation of 1, ensuring uniform feature scales for models like SVM.

Feature Engineering:
Created and transformed features based on initial findings to enhance the dataset's predictive power.
### Model Training and Performance
The raisin data classification project utilized two machine learning models: Random Forest and Support Vector Machine (SVM). After preprocessing and feature engineering, the models were trained and evaluated on the dataset.
The Random Forest model achieved an accuracy of 84%, leveraging its ensemble of decision trees to make robust predictions.
The SVM model, known for its effectiveness in high-dimensional spaces, outperformed Random Forest with an accuracy of 87%. 
This higher accuracy indicates SVM's superior capability in classifying the raisin types based on the given features.
### Dataset Description
The dataset comprises 900 rows and 7 columns, evenly split between two classes: Kecimen and Besni. Each class has 450 instances.
#### Column Information
Area: The number of pixels within the boundaries of the raisin.

Perimeter: The distance between the boundaries of the raisin and the pixels around it.

MajorAxisLength: The length of the main axis, which is the longest line that can be drawn on the raisin.

MinorAxisLength: The length of the minor axis, which is the shortest line that can be drawn on the raisin.

Eccentricity: A measure of the eccentricity of the ellipse that has the same moments as the raisin.

ConvexArea: The number of pixels in the smallest convex shell of the region formed by the raisin.

Extent: The ratio of the region formed by the raisin to the total pixels in the bounding box.

Class: The type of raisin, either Kecimen or Besni.
