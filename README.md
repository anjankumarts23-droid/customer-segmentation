# customer-segmentation
This project applies machine learning to group customers based on purchasing behavior. Using the Mall Customers dataset and K-Means clustering, it identifies distinct customer segments to help improve marketing strategies, personalization, and business decision-making.
 Introduction

Businesses often deal with a wide range of customers, each with unique purchase habits and preferences. Customer segmentation helps divide customers into meaningful groups for personalized marketing, strategy planning, and improving profit.
This project uses unsupervised learning, specifically K-Means clustering, to create distinct customer clusters based on demographic and spending variables.

 Problem Statement

Businesses need a way to categorize customers based on spending habits and income levels to better understand behavior and target marketing efforts effectively. The challenge is to build a clustering model that automatically identifies these groups.

 Objectives

To analyze customer demographic and spending data

To apply K-Means clustering for segmentation

To visualize clusters and understand customer behavior

To assist business decision-making with insights from segments

 Dataset Description

Dataset: Mall Customers Dataset
Columns:

CustomerID: Unique ID

Gender: Male/Female

Age: Customer age

Annual Income: Income in dollars

Spending Score: Assigned score (1–100) based on behavior

Samples: 200 rows

 Methodology
1. Data Loading & Cleaning

Load dataset using Pandas

Check for missing values

Clean and structure data

2. Feature Selection

Common feature combinations used:

Annual Income vs Spending Score

Age vs Spending Score

Age vs Income

3. Finding Optimal Number of Clusters

Using the Elbow Method, the value of k is selected based on minimizing Within-Cluster-Sum-of-Squares (WCSS).

4. Model Training

Algorithm used:

K-Means Clustering
Steps:

Fit the model

Predict cluster labels

Append cluster labels to the dataset

5. Cluster Visualization

Scatterplots are used to visualize:

Income vs Spending Score

Age vs Spending Score

Clusters with different colors

This helps identify clusters such as:

High income, high spenders

High income, low spenders

Low income, high spenders

Low income, low spenders

Younger or older groups

 Technologies Used

Python

Jupyter Notebook

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn (KMeans algorithm)

Implementation Summary

Import required libraries

Load dataset

Select features for clustering

Use Elbow Method to determine number of clusters

Train K-Means with optimal k

Predict clusters

Visualize the groups

Interpret cluster behavior

 Results & Observations

Typical clusters identified:

Cluster 1 – High Income, High Spenders

Premium customer group

High purchasing power

Cluster 2 – Low Income, Low Spenders

Budget-constrained consumers

Cluster 3 – High Income, Low Spenders

Potential customers to target with promotions

Cluster 4 – Low Income, High Spenders

Young customers with high spending behavior

Cluster 5 – Average Income, Average Spenders

Middle-segment customers

These insights help businesses create targeted marketing campaigns.

 Conclusion

The K-Means clustering model successfully segments customers into meaningful groups. These segments reveal spending behavior, income levels, and opportunities for personalized marketing. Customer segmentation enables businesses to make informed decisions and improve overall customer engagement.

 Future Enhancements

Use advanced clustering algorithms like DBSCAN or Hierarchical Clustering

Build a dashboard using Streamlit or Power BI

Apply PCA for dimensionality reduction

Add real-time segmentation on live data

 References

Scikit-learn Documentation

Mall Customer Dataset

Python Data Science Libraries
