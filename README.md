# Customer Segmentation using K-means Clustering

This project demonstrates customer segmentation using the **K-means clustering algorithm**, a popular unsupervised machine learning technique. The segmentation is based on a customer's annual income and spending score, using a dataset of mall customers (`Mall_Customers.csv`).

## Project Overview

The objective of this project is to categorize customers into different segments based on their purchasing behavior. This can help businesses understand customer needs and preferences, enabling them to optimize marketing strategies, customer engagement, and resource allocation.

## Dataset Description

The dataset `Mall_Customers.csv` contains 200 observations and the following features:

- **CustomerID**: A unique identifier for each customer.
- **Gender**: The customer's gender (Male/Female).
- **Age**: The age of the customer.
- **Annual Income (k$)**: The annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: A score assigned to customers based on their spending habits and purchasing behavior.

## Objective

The goal of this project is to apply **K-means clustering** to group customers into different segments based on their annual income and spending score. These groups can be used to:
- Identify different customer personas.
- Target specific segments for marketing campaigns.
- Improve customer retention and satisfaction.

## Methodology

### 1. Data Preprocessing
- The features **Annual Income** and **Spending Score** were selected for clustering.
- Data cleaning is minimal as the dataset is already well-structured.

### 2. Elbow Method
- To determine the optimal number of clusters, the **Elbow Method** is used by calculating the Within-Cluster Sum of Squares (WCSS) for a range of cluster values.
- The Elbow Method helps in identifying the ideal number of clusters by finding the point where the WCSS starts to diminish rapidly.

### 3. K-means Clustering
- After determining the optimal number of clusters, the **K-means algorithm** is applied to the data to form clusters.
- The centroids of each cluster are calculated, and customers are assigned to the closest centroid based on their income and spending score.

### 4. Visualization
- Scatter plots are used to visualize the clusters and centroids.
- Customers are represented as points, and the centroids of the clusters are marked to indicate the center of each group.

## Libraries Used

The following Python libraries are required to run the project:

- `pandas`: For data handling and manipulation.
- `matplotlib`: For plotting and visualization.
- `scikit-learn`: For applying the K-means clustering algorithm.


## Results

The results demonstrate that the customers were segmented into distinct groups. Each cluster represents a different customer segment based on their income and spending behavior. These clusters can be interpreted as different personas, such as:
- High-income, low-spending customers.
- Low-income, high-spending customers.
- Average-income, balanced-spending customers, etc.



