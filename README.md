# Dry_Bean_Dataset - Data preprocessing

1️ Dataset Source (Link)

The dataset used in this study is the Dry Bean Dataset from the UCI Machine Learning Repository:

🔗 https://archive.ics.uci.edu/ml/datasets/Dry+Bean+Dataset

It contains morphological measurements extracted from images of seven dry bean varieties:
Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, and Sira.

2️ Problem Statement
The objective was to Preprocess and Visualize the dataset.  The target variable is Class representing bean type and each bean sample is described using 16 numerical shape and size features such as:

- Area (A)

- Perimeter (P)

- Major axis length (L)

- Minor axis length (l)

- Aspect ratio (K)

- Eccentricity (Ec)

- Convex area (C)

- Equivalent diameter (Ed)

- Extent (Ex)

- Solidity (S)

- Roundness (R)

- Compactness (CO)

- ShapeFactor1–4 (SF1–SF4)

3 Summary of preprocessing decisions: 
✔ Data Cleaning
 -Duplicate rows were identified and removed.
 -No missing values were detected in the dataset.
 -Feature scaling and LAbel encoding performed

4 Key insights & observations: 

 -Several features contained a high number of IQR-based outliers.
-Size-related features (Area, Perimeter, MajorAxisLength, ConvexArea, EquivalentDiameter) showed strong positive skewness (>1).
-Shape-based features (Roundness, ShapeFactor, Solidity) showed strong negative skewness (< -2).
-RobustScaler was applied to reduce the effect of skewness and extreme values.
-Strong correlation exist between variables.

5 Potential Next Modeling Steps: 
Use advanced models such as Random forest and Gradient Boosting etc to develop a multi-class classification model that accurately predicts the bean variety (Class) based on its morphological features derived from image processing techniques.







