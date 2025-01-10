# Classification and Clustering models for Kickstarter projects
- Project for INSY446 - Data Mining for Business Analytics

## Introduction to Business Case
Kickstarter is a global crowdfunding platform that bridges the gap between creators and supporters. This project consists of two main components. The first focuses on developing a classification model to predict the likelihood of a project's success before its launch. This predictive tool aims to assist project owners by providing actionable insights into the optimal combination of attributes to maximize funding potential. The second component involves building a clustering model to categorize projects based on their characteristics. This model can serve various purposes, such as enabling Kickstarter staff to analyze project types on the platform, streamlining the verification process for new submissions, or identifying specific categories of projects that may require additional support or resources.

## Classification Model - Model Selection
The dataset is split into training and testing sets in 2:1 ratio, and modeled using different classification models including Artificial Neural Network, Random Forest, Logistic Regression, KNN, Classification Tree, and Gradient Boosting. Following this, hyperparameter tuning is done for each model using GridSearchCV. Random Forest model was selected with the best set of hyperparameters since it gave the highest accuracy of 74.9%.

| Classification Model    | Accuracy score                         |
|----------------------|------------------------------------------------|
| Artificial Neural Network              | 68.75%                |
| Random Forest          | 74.9% |
| Logistic Regression     | 67.9%|
| KNN          | 69.8%                |
| Classification Tree         | 73.4%|
| Gradient Boosting         | 73.9%                 |


## Classification Model - Insights
The features that are most important to predict the project success are project goal, category, duration between the project creation and launch, duration between the project launch and deadline, and length of the project name. Thus, a project owner should carefully evaluate these features of their project to maximize the chance of success.

## Clustering Model - Finding optimal number of clusters
To find the optimal number of clusters for the model, two approaches are used – PCA and K-Means Clustering

## Clustering Model - Insights
Cluster 1: Represents projects originating from the US, showing the dominance of US-based projects on Kickstarter.
Cluster 2: Includes projects from GB (Great Britain), indicating a smaller but significant contributor to the platform.
Cluster 3: Groups projects from all other countries combined, reflecting the diversity of international creators on Kickstarter.

The clustering highlights that the origin of the project country is a strong differentiating factor. It suggests that project attributes like funding success, category trends, or project scale may vary significantly by country.

The US has a disproportionately large share of projects, suggesting Kickstarter's strong market penetration in the US compared to other regions.
