# Multiclass-Bean-Classifier-ML
# **Dry Bean Classification using Machine Learning**

## **Dataset Overview**

**Dry Bean Dataset**

- Donation Date: 9/14/2020
- Number of Instances: 13,611
- Number of Attributes: 17
- Attribute Types: Integer, Real
- Subject Area: Computer
- Associated Tasks: Classification

**Dataset Characteristics**
- Multivariate
- Subject Area: Computer
- Associated Tasks: Classification
- Attribute Types: Integer, Real
- Number of Instances: 13,611
- Number of Attributes: 17

## **About the Dataset**

The dataset comprises images of 13,611 grains of 7 different registered dry beans, captured with a high-resolution camera. It includes 16 features, consisting of 12 dimensions and 4 shape forms obtained from the grains.

## **Attribute Information**

1. **Area (A):** The area of a bean zone and the number of pixels within its boundaries.
2. **Perimeter (P):** Bean circumference, defined as the length of its border.
3. **Major axis length (L):** The distance between the ends of the longest line that can be drawn from a bean.
4. **Minor axis length (l):** The longest line that can be drawn from the bean while standing perpendicular to the main axis.
5. **Aspect ratio (K):** Defines the relationship between L and l.
6. **Eccentricity (Ec):** Eccentricity of the ellipse having the same moments as the region.
7. **Convex area (C):** Number of pixels in the smallest convex polygon that can contain the area of a bean seed.
8. **Equivalent diameter (Ed):** The diameter of a circle having the same area as a bean seed area.
9. **Extent (Ex):** The ratio of the pixels in the bounding box to the bean area.
10. **Solidity (S):** Also known as convexity, the ratio of the pixels in the convex shell to those found in beans.
11. **Roundness (R):** Calculated with the formula: (4piA)/(P^2)
12. **Compactness (CO):** Measures the roundness of an object: Ed/L
13. **ShapeFactor1 (SF1)**
14. **ShapeFactor2 (SF2)**
15. **ShapeFactor3 (SF3)**
16. **ShapeFactor4 (SF4)**
17. **Class (Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, and Sira)

## **Reference Paper**

**Multiclass classification of dry beans using computer vision and machine learning techniques**

- Authors: Murat Koklu, Ilker Ali Ozkan
- Affiliation: Department of Computer Engineering, Selcuk University, Turkey, Konya, Turkey
- Published in: Computers and Electronics in Agriculture, 174
- [Read Paper](https://www.sciencedirect.com/science/article/abs/pii/S0168169919311573?via%3Dihub)


# **Implementation Overview**

## Data Loading and Exploration

The initial steps involve loading the Dry Bean dataset and exploring its characteristics:

1. **Import Libraries:** Necessary libraries, including pandas, numpy, and seaborn, are imported.

2. **Load Dataset:** The Dry Bean dataset is loaded into a Pandas dataframe using the `pd.read_csv` function.

3. **Missing Values Analysis:** A heatmap is generated to visualize missing values in the dataset. This helps in understanding the data quality and completeness.

4. **Class Distribution:** A countplot is created to visualize the distribution of different classes in the 'Class' variable, providing insights into the dataset's class balance.

5. **Data Visualization:** A histogram is plotted to visualize the dataset's distribution using 20 bins and a figure size of 15x15.

## Data Preprocessing

The following steps involve preparing the data for model training:

1. **Encode Class Labels:** The 'Class' variable is encoded using LabelEncoder to convert categorical labels into numerical values.

2. **Split Dataset:** The dataset is split into features (X) and the target variable (y). Further, the dataset is divided into training and testing sets using an 80:20 ratio.

## Model Training

Machine learning models are trained to predict the class labels of dry bean seeds:

1. **Extra Trees Classifier:** An Extra Trees classifier is trained with 500 estimators and a random state of 42. Feature importances are printed, and a bar plot visualizes the top 10 features.

2. **MLPClassifier (Neural Network):** An MLPClassifier model is trained with specific hyperparameters. Classification accuracy, error rate, and a confusion matrix are presented.

3. **Random Forest Classifier:** A RandomForestClassifier is trained with specified hyperparameters. Accuracy, error rate, and a classification report are provided.

4. **Support Vector Machine (SVM):** An SVM model with RBF kernel and specific hyperparameters is trained. Accuracy, error rate, and a classification report are displayed.

## Hyperparameter Tuning

For the MLPClassifier and SVM models, hyperparameter tuning is performed:

1. **Randomized Search (MLPClassifier):** RandomizedSearchCV is used for hyperparameter tuning, and the best hyperparameters along with the accuracy score are printed.

2. **SVM Hyperparameter Tuning:** Hyperparameters are fine-tuned using RandomizedSearchCV, and the best hyperparameters are displayed.

## Model Evaluation

The performance of the tuned models is evaluated on the test set (continued):

1. **MLPClassifier with Hyperparameter Tuning:** Accuracy, error rate, and a classification report are provided.

2. **SVM with Hyperparameter Tuning:** Accuracy, error rate, and a classification report are presented.

3. **Random Forest Classifier:** Accuracy, error rate, and a classification report are shown.

## Conclusion

The section concludes by highlighting the effectiveness of machine learning in dry bean classification. It summarizes findings, model performance, and the impact of hyperparameter tuning. Recommendations for future improvements are also discussed.

**Note: The complete code implementation can be found in the provided code file.**
## Important
# Machine Learning Coursework Assignment

This repository contains my solution for a Machine Learning coursework assignment as part of the Machine Learning module in Msc. Data Science at University of Sussex. The assignment was completed during the 2022-2023 year.

## Disclaimer
**Note to Course Instructors and Evaluators:**
This project represents my individual effort and understanding of the coursework requirements. It is submitted in fulfillment of the academic requirements for the Machine Learning module. The code and documentation are provided for educational purposes and as a showcase of my learning progress.

**Academic Integrity:**
I have adhered to the principles of academic integrity throughout the completion of this assignment. Any external resources, code snippets, or references used are appropriately cited in the code and documentation.

## Important Notice to Future Students
**Attention:** This project, including its code, documentation, and any associated materials, is the result of my individual effort and understanding. Future students are hereby informed not to copy or reproduce any part of this project. Such actions may be considered a violation of academic integrity policies, which could lead to severe consequences, including but not limited to disciplinary action by the university. I, the original author, will not be held responsible for any repercussions resulting from the misuse of this work by others. It is strongly advised to adhere to the principles of academic integrity and conduct your own work independently.

**Note:** Always refer to your university's policies on academic integrity and honor codes.


*Note: This README is designed to be transparent about the nature of the project and to comply with academic honesty policies.*
