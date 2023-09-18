# Breast Cancer Analysis and Prediction

## Introduction

Breast cancer is cancer that forms in the cells of the breasts.<p>It arises in the lining cells (epithelium) of the ducts (85%) or lobules (15%) in the glandular tissue of the breast. Initially, the cancerous growth is confined to the duct or lobule (“in situ”) where it generally causes no symptoms and has minimal potential for spread (metastasis).<br>
    
Most types of breast cancer are easy to diagnose by microscopic analysis of a sample - or biopsy - of the affected area of the breast. Also, there are types of breast cancer that require specialized lab exams.

## Dataset

We used the data published by UCI Machine Learning Repository, which consisted of features computed from digitized images of breast mass fine needle aspirates (FNAs). These features described characteristics of cell nuclei present in the images. The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius. This dataset is licenced under a [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode) (CC BY 4.0) license and can be find in [here](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic).

## Preprocessing

In this notebook at first we explored the data and then visulized the correlation between all features to undrestand it better. We even pairploted each 10 features (mean, starndard error and worst) and the diagnosis of them to see how seperable they are.
We used a simple preprocess, there was another column with all null values which we removed and then changed the target column from ['B','M'] to [0,1]. At last we used StandardScaler from sklearn library to standardize our features and then we splited data to train and test sets. 

## Models and Results

We used 4 classification models- Logistic Regression, K Nearest Neighbours, Random Forests and Support Vector Machines (SVM) to predict diagnosis of breast cancer data. We acheved 98 percent for accuracy.


